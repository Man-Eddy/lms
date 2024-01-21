<template>
    <div>
      <h3>Leave Requests List</h3>
      <ul>
        <li v-for="request in leaveRequests" :key="request.id">
          {{ request.employee }} - {{ request.type }} - {{ request.startDate }} to {{ request.endDate }} - Status: {{ request.status }}
        </li>
      </ul>
    </div>
  </template>
  
  <script setup>
  const props = defineProps(['leaveRequests']);
  </script>
  