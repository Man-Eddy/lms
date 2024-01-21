<template>
    <div>
      <h3>Leave Requests</h3>
      <ul>
        <li v-for="request in leaveRequests" :key="request.id">
          {{ request.employeeName }} - {{ request.leaveType }} ({{ request.startDate }} to {{ request.endDate }})
          <!-- Add additional details as needed -->
          <button @click="approveLeave(request.id)">Approve</button>
          <button @click="rejectLeave(request.id)">Reject</button>
        </li>
      </ul>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const leaveRequests = ref([
    // Example leave requests data, replace with actual data
    { id: 1, employeeName: 'John Doe', leaveType: 'Annual Leave', startDate: '2023-03-01', endDate: '2023-03-05' },
    { id: 2, employeeName: 'Jane Smith', leaveType: 'Sick Leave', startDate: '2023-03-10', endDate: '2023-03-12' },
  ]);
  
  function approveLeave(requestId) {
    // Logic to approve leave request
    console.log(`Leave request ${requestId} approved.`);
  }
  
  function rejectLeave(requestId) {
    // Logic to reject leave request
    console.log(`Leave request ${requestId} rejected.`);
  }
  </script>
  
  <style scoped>

  </style>
  