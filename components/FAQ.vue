<template>
    <section class="py-20">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold mb-8">Часто задаваемые вопросы</h2>
        <div class="space-y-4">
          <div v-for="faq in faqs" :key="faq.id" class="bg-white p-6 rounded-lg shadow-lg hover:bg-gray-50 transition-transform transform hover:scale-105">
            <h3 class="text-xl font-semibold mb-4">{{ faq.question }}</h3>
            <p class="text-gray-700">{{ faq.answer }}</p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const faqs = ref([
    {
      id: 1,
      question: 'Как записаться на курс?',
      answer: 'Вы можете записаться на курс через нашу платформу, выбрав нужный курс и нажав на кнопку "Записаться".'
    },
    // Добавьте больше вопросов и ответов
  ])
  </script>
  
  <style scoped>
/* Стиль вопросов и ответов */
.text-xl {
  color: #444;
}
</style>