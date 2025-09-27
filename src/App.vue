<template>
  <div class="container">
    <header>
      <h1>Registro de notas</h1>
      <nav>
        <button>Formularios</button>
        <button>Lista de estudiantes</button>
      </nav>
    </header>

    <main>
      <StudentForm />
      <StudentList />
    </main>
  </div>
</template>

<script>
import StudentForm from "./components/StudentForm.vue";
import StudentList from "./components/StudentList.vue";

export default {
  name: "App",
  components: {
    StudentForm,
    StudentList,
  },
};
</script>

<style scoped>
.container {
  width: 90%;
  margin: auto;
  font-family: Arial, sans-serif;
}

header {
  background: #f5f5f5;
  padding: 10px;
}

nav button {
  margin: 5px;
  padding: 8px 12px;
  cursor: pointer;
}
</style>
