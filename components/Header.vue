<template>
    <header class="header-section">
      <div class="container">
        <div class="header-content">
          <div class="logo-container">
            <a class="navbar-brand" href="/">
              <img src="@/assets/MP-logo.jpg" alt="MP Logo" class="logo" />
              <span class="logo-text">Leave Management System</span>
            </a>
          </div>
        </div>
      </div>
    </header>
  </template>
  
  <script setup>
  // You can add logic if needed
  </script>
  
  <style scoped>
  .header-section {
    height: 80px; /* Adjust the height as needed */
    width: 100%; /* Set the width to 100% */
    background-color: #f8f9fa; /* Add a background color if desired */
    padding: 10px 0; /* Add padding for spacing */
  }
  
  .header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .logo {
    height: 60px; /* Adjust the height as needed */
    margin-right: 10px; /* Add margin for spacing */
  }
  
  .logo-text {
    line-height: 60px; /* Align text vertically with the logo */
    font-weight: bold; /* Optionally make the text bold */
  }
  </style>
  