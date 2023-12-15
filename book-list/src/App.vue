<script setup>
import { reactive, ref } from 'vue'
// ref para primitivos
let count = ref(0)

// reactive para objetos
let courses = reactive([
  {
    title: 'javascript'
  },
  {
    title: 'React'
  },
  {
    title: 'Vue'
  }
])

let newCourse = { }

function increment(){
  count.value ++
}
function addCourse(){
  courses.push(newCourse)
  newCourse = { }
}
</script>

<template>
  <div>
    <h1>{{ count }}</h1>
    <button @click="increment">Incrementar</button><br>
    
  </div>
  <div>
    <h1>Lista de cursos</h1>
      <ul>
        <li v-for="(course, index) in courses" :key="index">
          {{ course.title }}
        </li>
      </ul>

      <input v-model="newCourse.title" type="text"><br> <br>
      <button @click="addCourse">Adicionar</button> <br> 
      
  </div>
  
</template>

<style scoped>
</style>
