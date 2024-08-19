<template>
    <section class="py-20 bg-gray-100">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold mb-8">Наш блог</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div v-for="post in posts" :key="post.id" class="bg-white p-4 rounded shadow">
            <img :src="post.image" alt="post.title" class="w-full h-40 object-cover rounded mb-4"/>
            <h3 class="text-xl font-semibold mb-2">{{ post.title }}</h3>
            <p class="text-gray-700 mb-4">{{ post.excerpt }}</p>
            <a :href="`/blog/${post.id}`" class="text-blue-500 hover:underline">Читать далее</a>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const posts = ref([
    {
      id: 1,
      title: 'Как выбрать курс по программированию?',
      excerpt: 'Советы и рекомендации для выбора идеального курса для вас.',
      image: '/images/blog1.jpg'
    },
    // Добавьте больше постов
  ])
  </script>
  