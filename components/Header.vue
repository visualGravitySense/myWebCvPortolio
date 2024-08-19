<template>
  <header class="bg-black text-white p-6 shadow-custom">
    <div class="container mx-auto flex items-center justify-between">
      <!-- Логотип -->
      <a href="/" class="text-4xl font-bold neon-text">
        LOGO
      </a>

      <!-- Навигация -->
      <nav>
        <ul class="flex space-x-6">
          <li>
            <a href="/courses" class="nav-link">Курсы</a>
          </li>
          <li>
            <a href="/about" class="nav-link">О нас</a>
          </li>
          <li>
            <a href="/contact" class="nav-link">Контакты</a>
          </li>
          <li>
            <a href="/login" class="nav-link">Вход</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script setup>
// В этом примере нет необходимости в скриптовой части
</script>

<style scoped>
/* Темный фон и эффект неона */
header {
  background-color: #000;
  color: #fff;
}

.shadow-custom {
  box-shadow: 0 0 15px rgba(0, 255, 0, 0.8);
}

.neon-text {
  color: #0f0;
  text-shadow: 0 0 5px rgba(0, 255, 0, 0.9),
               0 0 10px rgba(0, 255, 0, 0.7),
               0 0 15px rgba(0, 255, 0, 0.5);
}

.nav-link {
  font-family: 'Courier New', Courier, monospace;
  font-size: 1.25rem;
  text-decoration: none;
  color: #fff;
  transition: color 0.3s ease;
}

.nav-link:hover {
  color: #0f0;
  text-shadow: 0 0 5px rgba(0, 255, 0, 0.9),
               0 0 10px rgba(0, 255, 0, 0.7),
               0 0 15px rgba(0, 255, 0, 0.5);
}
</style>
