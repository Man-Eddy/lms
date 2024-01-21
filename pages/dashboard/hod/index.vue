<template>
    <div>
      <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
          <a class="navbar-brand" href="/">LMS</a>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">
                <nuxt-link to="/dashboard" class="nav-link">Dashboard</nuxt-link>
              </li>
              <li class="nav-item">
                <nuxt-link to="/dashboard/hod" class="nav-link">HOD Dashboard</nuxt-link>
              </li>
              <li class="nav-item">
                <nuxt-link to="/dashboard/leave-requests" class="nav-link">Leave Requests</nuxt-link>
              </li>
              <li class="nav-item">
                <nuxt-link to="/dashboard/employees" class="nav-link">Employee List</nuxt-link>
              </li>
            </ul>
          </div>
        </div>
      </nav>
  
      <div class="container mt-4">
        <h2>Head of Department Dashboard</h2>
        <LeaveRequestsList />
        <!-- Other HOD-specific content can be added here -->
      </div>
  
      <!-- Reusable Footer Component -->
      <Footer />
    </div>
  </template>
  
  <script setup>
  import LeaveRequestsList from '@/components/LeaveRequestsList.vue';
  import Footer from '@/components/Footer.vue';
  </script>
  
  <style scoped>
  /* Add custom styles if needed */
  </style>
  