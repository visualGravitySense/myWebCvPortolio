<template>
    <div class="container">
      <!-- <div class="profile"> -->
        <!-- <img :src="require('@/assets/img/profile-pic.jpg')" alt="Profile Picture" /> -->
        <!-- <img src="@/assets/img/profile-pic.jpg" alt="Profile Picture" />
        <h1>{{ name }}</h1>
        <h2>{{ role }}</h2>
        <p>{{ bio }}</p>
        <div class="social-links">
          <a v-for="link in socialLinks" :href="link.url" :key="link.platform">
            {{ link.platform }}
          </a>
        </div>
      </div> -->

      <!-- PROFILE  -->

      <!-- <div class="profile">
        <img src="@/assets/img/profile-pic.jpg" alt="Profile Picture" />
        <h1>{{ name }}</h1>
        <h2>{{ role }}</h2>
        <p>{{ bio }}</p>
        <div class="social-links">
          <a v-for="link in socialLinks" :href="link.url" :key="link.platform">
            {{ link.platform }}
          </a>
        </div>
      </div> -->

      <div class="profile">
        <img src="@/assets/img/profile-pic.jpg" alt="Profile Picture" />
        <h1>{{ name }}</h1>
        <h2>{{ role }}</h2>
        <p>{{ bio }}</p>
        <div class="social-links">

          <a href="https://github.com/visualGravitySense" target="_blank">
              <svg
                class="w-6 h-6 text-white-600 hover:text-gray-800 button--github"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                width="32"
                height="32"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path d="M12 2.247a10 10 0 0 0-3.162 19.487c.5.088.687-.212.687-.475c0-.237-.012-1.025-.012-1.862c-2.513.462-3.163-.613-3.363-1.175a3.636 3.636 0 0 0-1.025-1.413c-.35-.187-.85-.65-.013-.662a2.001 2.001 0 0 1 1.538 1.025a2.137 2.137 0 0 0 2.912.825a2.104 2.104 0 0 1 .638-1.338c-2.225-.25-4.55-1.112-4.55-4.937a3.892 3.892 0 0 1 1.025-2.688a3.594 3.594 0 0 1 .1-2.65s.837-.262 2.75 1.025a9.427 9.427 0 0 1 5 0c1.912-1.3 2.75-1.025 2.75-1.025a3.593 3.593 0 0 1 .1 2.65a3.869 3.869 0 0 1 1.025 2.688c0 3.837-2.338 4.687-4.563 4.937a2.368 2.368 0 0 1 .675 1.85c0 1.338-.012 2.413-.012 2.75c0 .263.187.575.687.475A10.005 10.005 0 0 0 12 2.247z" fill="" />
              </svg>
            </a>
            <a href="https://www.linkedin.com/in/dmitri-gornakov-7a664840/" target="_blank">
              <svg
                class="w-6 h-6 text-white-600 hover:text-blue-800 button--linkedin"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                width="32"
                height="32"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path d="M4.98 3.5c0 .92-.75 1.67-1.68 1.67H3.3c-.92 0-1.68-.75-1.68-1.67S2.38 1.83 3.3 1.83c.93 0 1.68.75 1.68 1.67zm.02 4.17H1v14h3.96v-14zm7.92 0H9v14h3.96v-7.64c0-3.64 4.81-3.94 4.81 0v7.64H21v-8.98c0-7.36-8.48-7.11-10.08-3.48V7.67h-.02z" fill="" />
              </svg>
            </a>

<!--             
          <a v-for="link in socialLinks" :href="link.url" :key="link.platform">
            {{ link.platform }}
          </a> -->
        </div>

        <div class="flex justify-center pt-4 space-x-2">

          <h2 class="text-2xl leading-7 font-semibold">Contact</h2>
        <p class="mt-3 text-gray-600 hover:text-purple-800">📧Email: <a href="mailto:dmitri.gornakov@gmail.com">dmitri.gornakov@gmail.com</a></p>
        <p class="mt-3 text-gray-600 hover:text-purple-800">☎️Phone: <a href="tel:+37258976398">+372 5897 6398</a></p>

            
          </div>

      </div>
  
      <!-- <div class="projects">
        <h3>Recent Projects</h3>
        <div class="project-list">
          <div v-for="project in projects" :key="project.name" class="project">
            <h4>{{ project.name }}</h4>
            <p>{{ project.description }}</p>
          </div>
        </div>
      </div>
  
      <div class="articles">
        <h3>Recent Articles</h3>
        <ul>
          <li v-for="article in articles" :key="article.title">
            <a :href="article.link">{{ article.title }}</a>
          </li>
        </ul>
      </div> -->

      <div class="projects">
        <h3>Recent Projects</h3>
        <div class="project-list">
          <div v-for="project in projects" :key="project.name" class="project">
            <h4>{{ project.name }}</h4>
            <p>{{ project.description }}</p>
          </div>
        </div>
      </div>

      <!-- <div class="articles">
        <h3>Recent Articles</h3>
        <ul>
          <li v-for="article in articles" :key="article.title">
            <a :href="article.link">{{ article.title }}</a>
          </li>
        </ul>
      </div> -->

      <div class="articles">
        <h3>Recent Articles</h3>
        <div class="article-list">
          <div v-for="article in articles" :key="article.title" class="article">
            <a :href="article.link" class="article-title">
              <h4>{{ article.title }}</h4>
              <p>{{ article.description }}</p>
            </a>
          </div>
        </div>

      </div>
            
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        profilePic: '@/assets/img/profile-pic.jpg',
        name: 'Dmitri Gornakov',
        role: 'Creative Technologist (UI/UX, Front-End & Back-End)',
        bio: 'I craft standout digital experiences by seamlessly blending UI/UX design, front-end expertise in Vue.js and React, and back-end mastery with Python. My diverse skill set allows me to build innovative, user-focused products from concept to code.',
        socialLinks: [
          { platform: 'Twitter', url: 'https://twitter.com/PhilippKief' },
          { platform: 'GitHub', url: 'https://github.com/PKief' }
        ],
        projects: [
          { name: 'Material Icon Theme', description: 'Icon theme for VS Code' },
          { name: 'Material Color Converter', description: 'Convert colors' }
        ],
        articles: [
          { title: 'Global Error Handling in Angular', link: '#', description: 'Description about artiles' },
          { title: 'Automatic Dark Mode Detection in Angular', link: '#', description: 'Description about artiles' }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .container {
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px;
    color: #0c0c0c;
  }
  .profile {
  background-color: #f4f4f4; /* Neutral light gray background */
  color: #333; /* Dark gray text for professionalism */
  padding: 40px;
  border: 2px solid #aaa; /* Subtle border for distinction */
  display: grid;
  grid-template-columns: 1fr 2fr; /* Asymmetric layout */
  gap: 20px;
  transform: rotate(-1deg); /* Slightly off balance for creative effect */
  max-width: 900px;
  margin: auto;
}

.profile img {
  width: 150px;
  border-radius: 50%; /* Soft rounded image for a modern feel */
  filter: grayscale(80%); /* Muted grayscale look */
  transform: rotate(5deg); /* Slight tilt for creative imbalance */
  margin-bottom: 20px;
  border: 5px solid #ddd;
}

h1 {
  font-size: 2.5rem;
  color: #333; /* Professional dark text */
  font-weight: bold;
  margin-bottom: 5px;
  letter-spacing: -0.5px;
  transform: rotate(-2deg); /* Slight text rotation for character */
}

h2 {
  font-size: 1.8rem;
  color: #555; /* Slightly lighter for a subtler contrast */
  font-style: italic;
  margin-top: 0;
}

p {
  font-size: 1.2rem;
  color: #666; /* Softer color for bio text */
  background-color: #eaeaea; /* Light background for distinction */
  padding: 15px;
  border-radius: 8px;
  text-align: left;
  border: 2px dashed #ccc;
}

.social-links {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 10px;
}

.social-links a {
  font-size: 1.2rem;
  text-decoration: none;
  color: #007bff; /* Calm blue for links */
  background-color: #f7f7f7;
  padding: 8px 12px;
  border-radius: 4px;
  border: 1px solid #ccc;
  transition: all 0.3s ease;
  /* transform: rotate(-1deg);  Subtle skew to match anti-design theme */
}

.social-links a:hover {
  color: #fff;
  background-color: #333; /* Professional hover effect */
  border-color: #333;
}

  /* .projects, .articles {
    margin-top: 50px;
  }
  .project-list {
    display: flex;
    justify-content: space-around;
  }
  .project {
    width: 200px;
    background-color: #222;
    padding: 20px;
    border-radius: 10px;
  } */

  /* Projects Block */
.projects {
  background-color: #f9f9f9; /* Neutral background */
  padding: 40px;
  border: 2px solid #ddd;
  margin: 40px 0;
  transform: rotate(-1deg); /* Subtle creative twist */
}

.projects h3 {
  font-size: 2rem;
  color: #444;
  letter-spacing: -0.5px;
  margin-bottom: 20px;
  transform: rotate(1deg); /* Small tilt for a creative feel */
}

.project-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); /* Flexible grid */
  gap: 20px;
}

.project {
  background-color: #eaeaea;
  border: 1px solid #ccc;
  padding: 20px;
  border-radius: 8px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  transform: rotate(-0.5deg); /* Slight tilt */
}

.project:hover {
  transform: scale(1.05) rotate(0deg); /* Smooth interaction */
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1);
}

.project h4 {
  font-size: 1.5rem;
  color: #333;
  margin-bottom: 10px;
  letter-spacing: -0.5px;
}

.project p {
  font-size: 1rem;
  color: #555;
  line-height: 1.5;
}

/* Articles Block */
.articles {
  background-color: #f5f5f5; /* Soft neutral background */
  padding: 50px;
  border: 2px solid #ddd;
  margin: 40px 0;
  transform: rotate(1deg); /* Slight rotation for creative touch */
}

.articles h3 {
  font-size: 2.2rem;
  color: #333;
  letter-spacing: -0.5px;
  margin-bottom: 30px;
  transform: rotate(-1deg); /* Creative tilt */
}

/* Article Card Grid */
.article-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); /* Responsive grid layout */
  gap: 30px;
}

/* Individual Article Card */
.article {
  background-color: #ffffff;
  border: 1px solid #ccc;
  padding: 20px;
  border-radius: 8px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  transform: rotate(-0.5deg); /* Slight creative rotation */
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.05); /* Subtle shadow */
}

.article:hover {
  transform: scale(1.05) rotate(0deg); /* Interactive hover effect */
  box-shadow: 0px 6px 14px rgba(0, 0, 0, 0.1); /* Enhanced shadow on hover */
}

/* Article Title and Description */
.article-title {
  text-decoration: none;
  color: inherit;
}

.article h4 {
  font-size: 1.5rem;
  color: #333;
  margin-bottom: 10px;
  letter-spacing: -0.5px;
}

.article p {
  font-size: 1rem;
  color: #666;
  line-height: 1.6;
  background-color: #f9f9f9;
  padding: 10px;
  border-radius: 4px;
  margin: 0;
}

/* Interactive Hover Effect for Article Links */
.article-title:hover h4 {
  color: #007bff;
}

.article-title:hover p {
  background-color: #f1f1f1;
}

  </style>
  

  

<!-- <template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
  </div>
</template> -->

<!-- <template>
  <div>
    
    <Header />
    <HeroSection />
    <FeaturedCourses />
    <NewArrivals />
    <FeaturedInstructors />
    <StudentReviews />
    <Blog />
    <FAQ />
    <Footer />
  </div>
</template>

<script setup>
import Header from '~/components/Header.vue'
import HeroSection from '~/components/HeroSection.vue'
import FeaturedCourses from '~/components/FeaturedCourses.vue'
import NewArrivals from '~/components/NewArrivals.vue'
import FeaturedInstructors from '~/components/FeaturedInstructors.vue'
import StudentReviews from '~/components/StudentReviews.vue'
import Blog from '~/components/Blog.vue'
import FAQ from '~/components/FAQ.vue'
import Footer from '~/components/Footer.vue'
</script> -->


