<template>
    <section class="py-20 bg-gray-50">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold mb-8">Новые поступления</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div v-for="item in newArrivals" :key="item.id" class="bg-white p-4 rounded shadow">
            <img :src="item.image" alt="item.title" class="w-full h-40 object-cover rounded mb-4"/>
            <h3 class="text-xl font-semibold mb-2">{{ item.title }}</h3>
            <p class="text-gray-700 mb-4">{{ item.description }}</p>
            <a :href="`/courses/${item.id}`" class="text-blue-500 hover:underline">Посмотреть</a>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const newArrivals = ref([
    {
      id: 1,
      title: 'Основы JavaScript',
      description: 'Изучите основы JavaScript, один из самых популярных языков программирования.',
      image: '/images/javascript-course.jpg'
    },
    {
      id: 2,
      title: 'Введение в Vue 3',
      description: 'Погружение в Vue 3, современный фреймворк для создания интерфейсов.',
      image: '/images/vue-course.jpg'
    },
    {
      id: 3,
      title: 'Продвинутый CSS',
      description: 'Углубленное изучение CSS для создания современных и отзывчивых веб-дизайнов.',
      image: '/images/css-course.jpg'
    },
    // Добавьте больше новых поступлений
  ])
  </script>
  