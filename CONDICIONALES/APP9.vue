
<script>
export default {
  data() {
    return {
      alumnos: [
        { nc: 22620001, nombre: 'ANGEL ATONIO LOPEZ PEREZ', carrera: 'Sistemas', gusto: 'futbol' },
        { nc: 22620002, nombre: 'KIMBERLY MENDOZA HERNANDEZ', carrera: 'Sistemas', gusto: 'ver tiktoks' },
        { nc: 22620003, nombre: 'ARCANGEL CRUZ GOINZALEZ', carrera: 'Sistemas', gusto: 'futbol' },
        { nc: 22620004, nombre: 'JUAN ANTONIO NICOLAS PEREZ', carrera: 'Sistemas', gusto: 'futbol' },
        { nc: 22620005, nombre: 'JOSUE VAZQUEZ RAMIREZ', carrera: 'Sistemas', gusto: 'futbol' },
        { nc: 22620006, nombre: 'ANTONIO ANGEL PEREZ LOPEZ', carrera: 'Sistemas', gusto: 'futbol' },
        { nc: 22620007, nombre: 'JOSÉ RAMÍREZ LÓPEZ', carrera: 'Docente', gusto: 'futbol' },
        { nc: 22620008, nombre: 'WILI PAUPAU', carrera: 'Docente', gusto: 'futbol' }
      ],
      searchQuery: ''
    };
  },
  computed: {
    filteredAlumnos() {
      const query = this.searchQuery.toLowerCase();
      return this.alumnos.filter(alumno =>
        alumno.nombre.toLowerCase().includes(query) ||
        alumno.nc.toString().includes(query) ||
        alumno.carrera.toLowerCase().includes(query) ||
        alumno.gusto.toLowerCase().includes(query)
      );
    }
  }
};
</script>

<template>
  <div class="container">
    <h1 class="titulo">Lista de Alumnos</h1>
    <div class="search-container">
      <input v-model="searchQuery" class="search-input" placeholder="Buscar...">
    </div>
    <div class="table-responsive">
      <table class="tabla">
        <thead>
          <tr>
            <th>No. Control</th>
            <th>Nombre</th>
            <th>Carrera</th>
            <th>Gusto</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="alumno in filteredAlumnos" :key="alumno.nc">
            <td>{{ alumno.nc }}</td>
            <td>{{ alumno.nombre }}</td>
            <td>{{ alumno.carrera }}</td>
            <td>{{ alumno.gusto }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style scoped>
body {
  background-image: url('https://m.media-amazon.com/images/I/51f2aXJBBqL.AC_UF894,1000_QL80.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  background-repeat: no-repeat;
  margin: 0;
  padding: 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  min-height: 100vh;
}

.container {
  max-width: 10000px;
  margin: 2rem auto;
  padding: 7rem;
  background: rgba(218, 11, 11, 0.9);
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
}

.titulo {
  color: #faf6f6;
  background-color: #0066cc;
  border-radius: 10px;
  padding: 1rem;
  margin-bottom: 1.5rem;
  font-size: 1.8rem;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.3);
}

.search-container {
  margin-bottom: 1.5rem;
}

.search-input {
  width: 100%;
  padding: 0.8rem 1rem;
  border: 2px solid #ddd;
  border-radius: 25px;
  font-size: 1rem;
  transition: all 0.3s ease;
}

.search-input:focus {
  outline: none;
  border-color: #0066cc;
  box-shadow: 0 0 0 3px rgba(0, 123, 255, 0.25);
}

.table-responsive {
  overflow-x: auto;
}

.tabla {
  width: 100%;
  border-collapse: separate;
  border-spacing: 0;
  margin-top: 1rem;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  overflow: hidden;
}

.tabla th, .tabla td {
  padding: 1rem;
  text-align: center;
  border: 1px solid #e0e0e0;
}

.tabla th {
  background-color: #0066cc;
  color: white;
  font-weight: 600;
  cursor: pointer;
  transition: background-color 0.2s;
}

.tabla th:hover {
  background-color: #0052a3;
}

.tabla tr:nth-child(even) {
  background-color: #f8f9fa;
}

.tabla tr:hover {
  background-color: #e9f5ff;
  transition: background-color 0.2s;
}

@media (max-width: 768px) {
  .container {
    padding: 1rem;
    margin: 1rem;
  }
  .tabla th, .tabla td {
    padding: 0.5rem;
    font-size: 0.9rem;
  }
}
</style>
