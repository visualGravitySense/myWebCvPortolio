<template>
    <section class="py-20 bg-gray-100">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold mb-8">Наши преподаватели</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div v-for="instructor in instructors" :key="instructor.id" class="bg-white p-4 rounded shadow">
            <img :src="instructor.image" alt="instructor.name" class="w-full h-40 object-cover rounded mb-4"/>
            <h3 class="text-xl font-semibold mb-2">{{ instructor.name }}</h3>
            <p class="text-gray-700 mb-4">{{ instructor.bio }}</p>
            <a :href="`/instructors/${instructor.id}`" class="text-blue-500 hover:underline">Посмотреть профиль</a>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const instructors = ref([
    {
      id: 1,
      name: 'Иван Иванов',
      bio: 'Эксперт по Vue.js и фронтенд-разработчик с 10-летним опытом.',
      image: '/images/instructor1.jpg'
    },
    // Добавьте больше преподавателей
  ])
  </script>
  