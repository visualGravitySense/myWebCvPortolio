<template>
    <section class="py-20">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold mb-8">Отзывы студентов</h2>
        <div class="space-y-8">
          <div v-for="review in reviews" :key="review.id" class="bg-white p-6 rounded shadow">
            <p class="text-gray-700 mb-4">“{{ review.text }}”</p>
            <p class="font-semibold">{{ review.studentName }}</p>
            <div class="flex items-center mt-2">
              <span v-for="n in review.rating" :key="n" class="text-yellow-400">★</span>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const reviews = ref([
    {
      id: 1,
      studentName: 'Мария Петрова',
      text: 'Этот курс был невероятно полезным для моего профессионального роста.',
      rating: 5
    },
    // Добавьте больше отзывов
  ])
  </script>
  