<script>
export default {
  data() {
    return {
      horarioAcademico: [
        {
          hora: '7:00 - 8:00',
          lunes: 'Programación Python',
          martes: 'Matemáticas Discretas',
          miercoles: 'Programación Python',
          jueves: 'Matemáticas Discretas',
          viernes: 'Taller de Radio'
        },
        {
          hora: '8:00 - 9:00',
          lunes: 'Bases de Datos',
          martes: 'Física',
          miercoles: 'Bases de Datos',
          jueves: 'Física',
          viernes: 'Club de Lectura'
        },
        {
          hora: '9:00 - 10:00',
          lunes: 'Inglés Técnico',
          martes: 'Algoritmos',
          miercoles: 'Inglés Técnico',
          jueves: 'Algoritmos',
          viernes: 'Gimnasio'
        },
        {
          hora: '10:00 - 11:00',
          lunes: 'Redes de Computadoras',
          martes: 'Ética Profesional',
          miercoles: 'Redes de Computadoras',
          jueves: 'Ética Profesional',
          viernes: 'Proyectos Personales'
        },
        {
          hora: '11:00 - 12:00',
          lunes: 'Taller de Investigación',
          martes: 'Taller de Investigación',
          miercoles: 'Taller de Investigación',
          jueves: 'Taller de Investigación',
          viernes: 'Videojuegos Educativos'
        }
      ],
      actividadesExtracurriculares: [
        {
          dia: 'Lunes',
          actividad: 'Club de Locución y Radio',
          participantes: 'Arcangel González',
          hora: '16:00 - 18:00'
        },
        {
          dia: 'Martes',
          actividad: 'Grupo de Lectura',
          participantes: 'Sofía Martínez',
          hora: '17:00 - 19:00'
        },
        {
          dia: 'Miércoles',
          actividad: 'Hackathons y Programación',
          participantes: 'Carlos Eduardo Torres',
          hora: '15:00 - 18:00'
        },
        {
          dia: 'Jueves',
          actividad: 'Club de Música',
          participantes: 'Mariana Fernández',
          hora: '16:00 - 18:00'
        },
        {
          dia: 'Viernes',
          actividad: 'Torneos de Videojuegos',
          participantes: 'Ricardo Gómez',
          hora: '14:00 - 17:00'
        },
        {
          dia: 'Sábado',
          actividad: 'Grupo de Fitness',
          participantes: 'Valeria Sánchez',
          hora: '9:00 - 11:00'
        }
      ],
      activeTab: 'academico'
    }
  },
  methods: {
    setActiveTab(tab) {
      this.activeTab = tab
    }
  }
}
</script>

<template>
  <div class="horario-container">
    <h1 class="titulo-horario">Horario Estudiantil</h1>
    
    <div class="tabs">
      <button 
        @click="setActiveTab('academico')" 
        :class="{ active: activeTab === 'academico' }"
      >
        Horario Académico
      </button>
      <button 
        @click="setActiveTab('extracurriculares')" 
        :class="{ active: activeTab === 'extracurriculares' }"
      >
        Actividades Extracurriculares
      </button>
    </div>
    
    <div v-if="activeTab === 'academico'" class="tabla-container">
      <table class="tabla-horario">
        <thead>
          <tr>
            <th>Hora</th>
            <th>Lunes</th>
            <th>Martes</th>
            <th>Miércoles</th>
            <th>Jueves</th>
            <th>Viernes</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(clase, index) in horarioAcademico" :key="index">
            <td>{{ clase.hora }}</td>
            <td>{{ clase.lunes }}</td>
            <td>{{ clase.martes }}</td>
            <td>{{ clase.miercoles }}</td>
            <td>{{ clase.jueves }}</td>
            <td>{{ clase.viernes }}</td>
          </tr>
        </tbody>
      </table>
    </div>
    
    <div v-if="activeTab === 'extracurriculares'" class="tabla-container">
      <table class="tabla-actividades">
        <thead>
          <tr>
            <th>Día</th>
            <th>Actividad</th>
            <th>Participantes Recomendados</th>
            <th>Hora</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(actividad, index) in actividadesExtracurriculares" :key="index">
            <td>{{ actividad.dia }}</td>
            <td>{{ actividad.actividad }}</td>
            <td>{{ actividad.participantes }}</td>
            <td>{{ actividad.hora }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style scoped>
.horario-container {
  max-width: 1200px;
  margin: 2rem auto;
  padding: 2rem;
  background: rgba(255, 255, 255, 0.95);
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.titulo-horario {
  color: #0066cc;
  text-align: center;
  margin-bottom: 1.5rem;
  font-size: 2rem;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
}

.tabs {
  display: flex;
  justify-content: center;
  margin-bottom: 2rem;
  gap: 1rem;
}

.tabs button {
  padding: 0.8rem 1.5rem;
  border: none;
  background-color: #e0e0e0;
  border-radius: 25px;
  cursor: pointer;
  font-weight: 600;
  transition: all 0.3s ease;
}

.tabs button.active {
  background-color: #0066cc;
  color: white;
}

.tabs button:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.tabla-container {
  overflow-x: auto;
}

.tabla-horario, .tabla-actividades {
  width: 100%;
  border-collapse: collapse;
  margin-top: 1rem;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
  border-radius: 10px;
  overflow: hidden;
}

.tabla-horario th, 
.tabla-horario td,
.tabla-actividades th,
.tabla-actividades td {
  padding: 1rem;
  text-align: center;
  border: 1px solid #e0e0e0;
}

.tabla-horario th,
.tabla-actividades th {
  background-color: #0066cc;
  color: white;
  font-weight: 600;
}

.tabla-horario tr:nth-child(even),
.tabla-actividades tr:nth-child(even) {
  background-color: #f8f9fa;
}

.tabla-horario tr:hover,
.tabla-actividades tr:hover {
  background-color: #e9f5ff;
}

@media (max-width: 768px) {
  .horario-container {
    padding: 1rem;
    margin: 1rem;
  }
  
  .tabs {
    flex-direction: column;
    align-items: center;
  }
  
  .tabla-horario th, 
  .tabla-horario td,
  .tabla-actividades th,
  .tabla-actividades td {
    padding: 0.5rem;
    font-size: 0.9rem;
  }
}
</style>