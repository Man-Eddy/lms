<template>
    <div>
      <Header />
  
      <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
          <a class="navbar-brand" href="/">LMS</a>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">

                <nuxt-link to="/auth/login" class="nav-link">Login</nuxt-link>
              </li>
              <li class="nav-item">
                <nuxt-link to="/dashboard" class="nav-link">Dashboard</nuxt-link>
              </li>
            </ul>
          </div>
        </div>
      </nav>
  
      <div class="container mt-4">
        <v-btn>
          Checking
        </v-btn>
        <h2>Login Page</h2>
        <LoginForm />
      </div>
  
      <!-- Inserting Footer Component -->
    </div>
    <Footer />
  </template>
  
  <script>
  import LoginForm from '@/components/auth/LoginForm.vue';
  import Footer from '@/components/Footer.vue'; // Adjust the path according to your project structure
  
  export default {
    components: {
      LoginForm,
      Footer,
    },
  };
  </script>
  