<template>
  <div>
    <!-- Header Section -->
    <header class="bg-light p-3">
      <div class="container">
        <h1>LMS Dashboard</h1>
      </div>
    </header>

    <!-- Navigation Menu -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container">
        <a class="navbar-brand" href="/">LMS</a>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <nuxt-link to="/dashboard" class="nav-link">Dashboard</nuxt-link>
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

    <!-- Main Content -->
    <div class="container mt-4">
      <LeaveRequestForm />

    </div>

    <!-- Footer Section -->
    <Footer />
  </div>
</template>

<script setup>
import LeaveRequestForm from '@/components/LeaveRequestForm.vue';
import Footer from '@/components/Footer.vue';
</script>

<style scoped>
</style>
