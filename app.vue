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

      <div class="hero-section">

        <div class="skills-section">
          <div class="inline-badge">UI/UX Design</div>
          <div class="blue-badge">Front-End</div>
          <div class="star-badge">Back-End</div>
          <div class="black-badge">Expertise in Vue<br>and React</div>
          <div class="yellow-badge">Back-end mastery<br>with Python</div>
          <span class="email-emoji"><a class="emoji-link" href="mailto:dmitri.gornakov@gmail.com">📧</a></span>
          <span class="phone-emoji"><a class="emoji-link" href="tel:+37258976398">☎️</a></span>
          <div class="social-links">
            <div class="git-ico"><Gitico/></div>
            <div class="in-ico"><Inico/></div>
          </div>
        
      </div>
        
        <img src="@/assets/img/profile-pic.jpg" alt="Profile Picture" class="profile-pic" />
          <h1 class="headline">Dmitri Gornakov</h1>
          <h2 class="sub-headline">CREATIVE <span class="highlight">TECHNOLOGIST</span></h2>
        
        <div class="content-wrapper">
          
          <p class="paragraph">I craft standout digital experiences by seamlessly blending UI/UX design, front-end expertise in Vue.js and React, and back-end mastery with Python. My diverse skill set allows me to build innovative, user-focused products from concept to code.</p>
        </div>        
        <!-- <img src="@/assets/img/profile-pic.jpg" alt="Profile Picture" class="profile-pic" /> -->
        <br>
        <a href="mailto:dmitri.gornakov@gmail.com" class="btn-primary">Hire Me</a>

      </div>

      

      <div class="profile">
        <!-- <img src="@/assets/img/profile-pic.jpg" alt="Profile Picture" />  -->
        <h1>{{ name }}</h1>
        <h2>{{ role }}</h2>
        <p>{{ bio }}</p>
        <div class="social-links">

          
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
            <h4>
              <a :href="project.url" target="_blank">{{ project.name }}</a>
            </h4>
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
  import Gitico from '~/components/UI/Gitico.vue'
  import Inico from '~/components/UI/Inico.vue'
  // import Header from '~/components/Header.vue'
  export default {
    components: { Gitico, Inico },
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
          { 
            name: 'edTech online education platform', 
            description: 'An edtech platform is a digital tool that provides interactive and accessible learning experiences.', 
            url: 'https://github.com/visualGravitySense/bisonWese-edTech'
          },
          { 
            name: 'Aawra service for beauty salons', 
            description: 'Offering a comprehensive suite of tools to streamline operations and enhance customer experiences.', 
            url: 'https://github.com/visualGravitySense/aawraOnline'
          },
          { 
            name: 'Website for car driving school', 
            description: 'The website is designed to increase bookings and enhance customer satisfaction.', 
            url: 'https://github.com/visualGravitySense/CarDrivingSchool'
          },
          
        ],
        articles: [
          { title: 'Tailwind CSS vs. Bootstrap', link: '#', description: 'A Comparison of Approaches — Flexibility vs. Pre-Built Solutions.' },
          { title: 'Tailwind CSS: A Revolution in Web Application Styling', link: '#', description: 'A Comparison of Approaches — Flexibility vs. Pre-Built Solutions' },
          { title: 'Why UI/UX Design Can Actually Break a Product', link: '#', description: "Today, UI/UX design is often seen as crucial to a product's success. However, in the pursuit of perfect interfaces, many companies lose sight of the primary goal." }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .container {
  background-color: #0c0c0c; /* Dark background */
  color: #fff; /* White text */
  padding: 20px;
}

.hero-section {
  position: relative; /* Чтобы внутри можно было использовать абсолютное позиционирование */
  text-align: center;
  padding: 50px 0;
}

.headline {
  font-size: 3rem;
  font-weight: bold;
  color: #fff;
}

.highlight {
  color: #d4ff00; /* Neon yellow/green */
  text-decoration: underline;
}

.sub-headline {
  font-size: 1.5rem;
  color: #ddd;
  margin: 20px 0;
}



.profile-pic {
  z-index: 1;
  border-radius: 50%;
  width: 150px;
  filter: grayscale(100%);
  margin: 20px 0;
  border: 5px solid #ddd;
}

.btn-primary {
  background-color: #d4ff00;
  color: #0c0c0c;
  padding: 10px 20px;
  text-decoration: none;
  font-weight: bold;
  border-radius: 4px;
  transition: background-color 0.3s ease;
}

.btn-primary:hover {
  background-color: #b2e600;
}

.skills-section {
  position: relative; /* Создает контекст для абсолютного позиционирования */
  z-index: 2;
}

.inline-badge {
    position: absolute;
    top: 15px; /* Позиция сверху */
    left: 150px; /* Позиция слева */
    border: 2px solid #f0eaea;
    color: #f0eaea;
    padding: 5px 10px;
    border-radius: 5px;
    background-color: transparent;
    font-weight: bold;
    font-size: 1.5rem;
    transform: rotate(-7deg); /* Поворот на 7 градусов влево */
}

.blue-badge {
    position: absolute;
    top: 100px;
    left: 300px;
    background-color: #5ceee9;
    color: #070707;
    padding: 5px 10px;
    border-radius: 5px;
    font-weight: bold;
    font-size: 1.5rem;
    transform: rotate(10deg); /* Поворот на 7 градусов влево */
}

.star-badge {
    position: absolute;
    top: 250px;
    left: 200px;
    background-color: #ffcc00;
    color: #070707;
    width: 100px;
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    clip-path: polygon(
    50% 0%, 85% 15%, 100% 50%, 85% 85%, 50% 100%,
    15% 85%, 0% 50%, 15% 15%);
    font-size: 1.5rem;
    transform: rotate(10deg); /* Поворот на 7 градусов влево */
    font-weight: bold;
}

.black-badge {
    position: absolute;
    top: 30px;
    right: 400px;
    background-color: #6cffae;
    color: #070707;
    padding: 5px 10px;
    border-radius: 5px;
    font-weight: bold;
    font-size: 1.5rem;
    transform: rotate(-10deg); /* Поворот на 7 градусов влево */
}

.yellow-badge {
    position: absolute;
    top: 250px;
    right: 150px;
    background-color: #ffb73b;
    color: #000;
    padding: 5px 10px;
    border-radius: 5px;
    font-weight: bold;
    font-size: 1.5rem;
    transform: rotate(7deg); /* Поворот на 7 градусов влево */
}

.emoji-link {
  text-decoration: none;
}

.email-emoji {
  position: absolute;
  top: 200px;
  left: 400px;
  transform: rotate(-10deg); /* Поворот на 7 градусов влево */
  font-size: 70px; /* Размер эмодзи */
  filter: hue-rotate(320deg);  
  display: inline-block; /* Чтобы применить фильтры */
  }


.phone-emoji {
  position: absolute;
  top: 170px;
  right: 375px;
  transform: rotate(-10deg); /* Поворот на 7 градусов влево */
  font-size: 80px; /* Размер эмодзи */
  filter: hue-rotate(320deg);
  display: inline-block; /* Чтобы применить фильтры */
}

.git-ico {
  position: absolute;
    top: 100px;
    right: 250px;
    background-color: #f7f7f7;
    color: #000;
    padding: 5px 10px;
    border-radius: 5px;
    font-weight: bold;
    transform: rotate(8deg); /* Поворот на 7 градусов влево */

}

.in-ico {
  position: absolute;
    top: 50px;
    left: 500px;
    background-color: #007bff;
    color: #000;
    padding: 5px 10px;
    border-radius: 5px;
    font-weight: bold;
    transform: rotate(-7deg); /* Поворот на 7 градусов влево */

}

/* .in-ico:hover {
  color: #fff;
} */

/* .social-links a:hover {
  color: #fff;
  background-color: #333; 
  border-color: #333;
} */


.skill-badge:hover {
  transform: scale(1.1);
  .profile {
  background-color: #f4f4f4; /* Neutral light gray background */
  color: #333; /* Dark gray text for professionalism */
  padding: 40px;
  border: 2px solid #aaa; /* Subtle border for distinction */
  display: grid;
  grid-template-columns: 1fr 2fr; /* Asymmetric layout */
  gap: 20px;
  /* transform: rotate(-1deg);  Slightly off balance for creative effect */
  max-width: 900px;
  margin: auto;
}
}

.profile img {
  width: 150px;
  border-radius: 50%; /* Soft rounded image for a modern feel */
  filter: grayscale(80%); /* Muted grayscale look */
  /*transform: rotate(5deg);  Slight tilt for creative imbalance */
  margin-bottom: 20px;
  border: 5px solid #ddd;
}

h1 {
  font-size: 2.5rem;
  color: #333; /* Professional dark text */
  font-weight: bold;
  margin-bottom: 5px;
  letter-spacing: -0.5px;
  /*transform: rotate(-2deg);  Slight text rotation for character */
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
  font-size: 3.2rem;
  text-decoration: none;
  /* color: #007bff; Calm blue for links */
  /* background-color: #f7f7f7; */
  padding: 8px 12px;
  /* border-radius: 4px; */
  /* border: 1px solid #ccc; */
  transition: all 0.3s ease;
  /* transform: rotate(-1deg);  Subtle skew to match anti-design theme */
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
  /*transform: rotate(-1deg);  Subtle creative twist */
}

.content-wrapper {
    max-width: 800px; /* Controls the maximum width of the block */
    margin: 0 auto; /* Centers the block horizontally */
    padding: 20px; /* Adds some padding around the text */
    text-align: center; /* Optional: centers the text within the block */
}

.paragraph {
    font-size: 1.2rem; /* Adjusts the font size */
    color: #f9f9f9; /* Text color */
    line-height: 1.6; /* Line spacing */
    background-color: unset;
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
  /*transform: rotate(-0.5deg);  Slight tilt */
}

.project:hover {
  transform: scale(1.05) rotate(-0.5deg); /* Smooth interaction */
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
  /*transform: rotate(1deg);  Slight rotation for creative touch */
}

.articles h3 {
  font-size: 2.2rem;
  color: #333;
  letter-spacing: -0.5px;
  margin-bottom: 30px;
   /*transform: rotate(-1deg); Creative tilt */
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
  /*transform: rotate(-0.5deg);  Slight creative rotation */
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.05); /* Subtle shadow */
}

.article:hover {
  transform: scale(1.05) rotate(-0.5deg); /* Interactive hover effect */
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

/* .article p {
  font-size: 1rem;
  color: #666;
  line-height: 1.6;
  background-color: #f9f9f9;
  padding: 10px;
  border-radius: 4px;
  margin: 0;
} */

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


