<template>
    <div>
      <h2>HR Registration Form</h2>
      <form @submit.prevent="submitRegistration">
        <!-- Employee Information -->
        <div class="mb-3">
          <label for="employeeID" class="form-label">Employee ID:</label>
          <input v-model="employeeID" type="text" class="form-control" id="employeeID" required>
        </div>
  
        <div class="mb-3">
          <label for="userID" class="form-label">User ID:</label>
          <input v-model="userID" type="text" class="form-control" id="userID" required>
        </div>
  
        <div class="mb-3">
          <label for="firstName" class="form-label">First Name:</label>
          <input v-model="firstName" type="text" class="form-control" id="firstName" required>
        </div>
  
        <div class="mb-3">
          <label for="lastName" class="form-label">Last Name:</label>
          <input v-model="lastName" type="text" class="form-control" id="lastName" required>
        </div>
  
        <div class="mb-3">
          <label for="email" class="form-label">Email:</label>
          <input v-model="email" type="email" class="form-control" id="email" required>
        </div>
  
        <div class="mb-3">
          <label for="position" class="form-label">Position:</label>
          <input v-model="position" type="text" class="form-control" id="position" required>
        </div>
  
        <!-- Account Type Dropdown -->
        <div class="mb-3">
          <label for="accountType" class="form-label">Account Type:</label>
          <select v-model="accountType" class="form-select" required>
            <option value="employee">Employee</option>
            <option value="hod">Head of Department (HOD)</option>
            <option value="oaf">Assistance Officer of Finance (OAF)</option>
          </select>
        </div>
  
        <button type="submit" class="btn btn-primary">Register</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        employeeID: '',
        userID: '',
        firstName: '',
        lastName: '',
        email: '',
        position: '',
        accountType: 'employee', // Default to employee account type
      };
    },
    methods: {
      submitRegistration() {
        // Logic to submit the registration
        console.log('Submitting registration:', this.employeeID, this.userID, this.firstName, this.lastName, this.email, this.position, this.accountType);
        // You can make an API request or perform any other necessary actions here
      },
    },
  };
  </script>
  
  <style scoped>
  /* Add custom styles if needed */
  </style>
  