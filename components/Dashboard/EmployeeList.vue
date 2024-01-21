<template>
    <div>
      <h2>Employee List</h2>
      <ul>
        <li v-for="employee in employeeList" :key="employee.id">
          <span>{{ employee.fullName }}</span>
          <span>{{ employee.position }}</span>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        employeeList: [
          { id: 1, fullName: 'John Doe', position: 'Software Engineer' },
          { id: 2, fullName: 'Jane Doe', position: 'Project Manager' },
          // Add more employees as needed
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add custom styles if needed */
  </style>
  