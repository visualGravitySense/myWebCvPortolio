<template>
    <footer class="bg-gray-800 text-white py-10">
      <div class="container mx-auto">
        <div class="flex flex-col md:flex-row md:justify-between">
          <div class="mb-6 md:mb-0">
            <a href="/" class="text-2xl font-bold mb-4 block">Logo</a>
            <p class="text-gray-400">Образовательная платформа для изучения новых навыков и повышения квалификации.</p>
          </div>
          <div class="mb-6 md:mb-0">
            <h3 class="text-lg font-semibold mb-4">Меню</h3>
            <ul>
              <li><a href="/about" class="hover:underline">О нас</a></li>
              <li><a href="/contact" class="hover:underline">Контакты</a></li>
              <li><a href="/courses" class="hover:underline">Курсы</a></li>
              <li><a href="/faq" class="hover:underline">Часто задаваемые вопросы</a></li>
            </ul>
          </div>
          <div class="mb-6 md:mb-0">
            <h3 class="text-lg font-semibold mb-4">Следите за нами</h3>
            <div class="flex space-x-4">
              <a href="https://facebook.com" class="text-gray-400 hover:text-white" aria-label="Facebook">
                <svg fill="currentColor" viewBox="0 0 24 24" class="w-6 h-6"><path d="M22 12h-4v8h-4v-8h-4v-4h4v-2c0-4.41 3.59-8 8-8h4v4h-4c-2.21 0-4 1.79-4 4v2h4l-2 4z"/></svg>
              </a>
              <a href="https://twitter.com" class="text-gray-400 hover:text-white" aria-label="Twitter">
                <svg fill="currentColor" viewBox="0 0 24 24" class="w-6 h-6"><path d="M23 3a10.92 10.92 0 01-3.14.86A5.45 5.45 0 0022.43 2a10.86 10.86 0 01-3.41 1.3A5.35 5.35 0 0016.5 2a5.41 5.41 0 00-5.44 5.45c0 .42.05.83.13 1.24A15.34 15.34 0 013 4.09a5.35 5.35 0 001.67 7.16A5.39 5.39 0 012 11v.07a5.34 5.34 0 004.3 5.28A5.41 5.41 0 014 16a5.43 5.43 0 004.57-2.13A10.71 10.71 0 0112 17c-2.5 0-4.83-.85-6.7-2.26A15.22 15.22 0 0012 20a15.5 15.5 0 0015-15.43c0-.23-.01-.45-.02-.67A10.8 10.8 0 0023 3z"/></svg>
              </a>
              <a href="https://instagram.com" class="text-gray-400 hover:text-white" aria-label="Instagram">
                <svg fill="currentColor" viewBox="0 0 24 24" class="w-6 h-6"><path d="M12 2.2c3.4 0 3.8.01 5.2.08 1.4.08 2.8.32 4 1.02 1.2.71 2.07 1.77 2.78 2.78.71 1.2.94 2.6 1.02 4 .07 1.4.07 1.8.07 5.2.07 3.4 0 3.8-.01 5.2-.08 1.4-.07 2.8-.32 4-1.02 1.2-.71 2.07-1.77 2.78-2.78.71-1.2.94-2.6 1.02-4 .07-1.4.07-1.8.07-5.2 0-3.4-.01-3.8-.08-5.2-.08-1.4-.32-2.8-1.02-4-1.2-1.2-2.07-2.07-2.78-2.78-.71-1.2-2.6-1.8-4-1.8-1.4-.07-1.8-.07-5.2-.07-3.4 0-3.8.01-5.2.07-1.4.07-2.8.32-4 1.02-1.2.71-2.07 1.77-2.78 2.78-.71 1.2-.94 2.6-1.02 4-.07 1.4-.07 1.8-.07 5.2 0 3.4.01 3.8.08 5.2.08 1.4.32 2.8 1.02 4 1.2 1.2 2.07 2.07 2.78 2.78.71 1.2 2.6 1.8 4 1.8 1.4.07 1.8.07 5.2.07 3.4 0 3.8-.01 5.2-.07 1.4-.07 2.8-.32 4-1.02 1.2-.71 2.07-1.77 2.78-2.78.71-1.2.94-2.6 1.02-4 .07-1.4.07-1.8.07-5.2 0-3.4-.01-3.8-.07-5.2-.08-1.4-.32-2.8-1.02-4-1.2-1.2-2.07-2.07-2.78-2.78-.71-1.2-2.6-1.8-4-1.8-1.4-.07-1.8-.07-5.2-.07zM12 5.9a6.1 6.1 0 106.1 6.1A6.1 6.1 0 0012 5.9zm0 10.4a4.3 4.3 0 114.3-4.3A4.3 4.3 0 0112 16.3zm6.8-9.8c.5 0 .9-.4.9-.9s-.4-.9-.9-.9-.9.4-.9.9.4.9.9.9z"/></svg>
              </a>
            </div>
          </div>
        </div>
        <div class="mt-10 border-t border-gray-700 pt-6 text-center">
          <p class="text-gray-400 text-sm">
            &copy; {{ new Date().getFullYear() }} Ваше название компании. Все права защищены.
          </p>
          <div class="mt-2">
            <a href="/privacy-policy" class="text-gray-400 hover:text-white mx-2">Политика конфиденциальности</a>
            |
            <a href="/terms-of-service" class="text-gray-400 hover:text-white mx-2">Условия использования</a>
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <style scoped>
  footer {
    border-top: 3px solid #ff0077; /* Яркая граница для акцента */
  }
  </style>
  