<template>
    <section class="py-20">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold mb-8">Популярные курсы</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div v-for="course in courses" :key="course.id" class="bg-white p-4 rounded shadow">
            <img :src="course.image" alt="course.title" class="w-full h-40 object-cover rounded mb-4"/>
            <h3 class="text-xl font-semibold mb-2">{{ course.title }}</h3>
            <p class="text-gray-700 mb-4">{{ course.description }}</p>
            <a :href="`/courses/${course.id}`" class="text-blue-500 hover:underline">Посмотреть курс</a>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const courses = ref([
    {
      id: 1,
      title: 'Курс по Vue.js',
      description: 'Изучите Vue.js с нуля',
      image: '/images/vue-course.jpg'
    },
    // Добавьте больше курсов
  ])
  </script>
  