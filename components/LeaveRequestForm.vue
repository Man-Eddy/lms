<template>
    <div>
      
      <form @submit.prevent="submitLeaveRequest">
        <div class="mb-3">
          <label for="leaveType" class="form-label">Leave Type:</label>
          <select v-model="leaveType" class="form-select" id="leaveType" required>
            <option value="annual">Annual Leave</option>
            <option value="sick">Sick Leave</option>
            <option value="materinity">Materinity Leave</option>
            <option value="">Circumstantial Leave</option>
           
          </select>
        </div>
        <div class="mb-3">
          <label for="startDate" class="form-label">Start Date:</label>
          <input v-model="startDate" type="date" class="form-control" id="startDate" required>
        </div>
        <div class="mb-3">
          <label for="endDate" class="form-label">End Date:</label>
          <input v-model="endDate" type="date" class="form-control" id="endDate" required>
        </div>
        <button type="submit" class="btn btn-primary">Submit Request</button>
      </form>

      

    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        leaveType: 'annual',
        startDate: '',
        endDate: '',
      };
    },
    methods: {
      submitLeaveRequest() {
        // Add logic to submit the leave request
        console.log('Submitting leave request:', this.leaveType, this.startDate, this.endDate);
        // You can make an API request or perform any other necessary actions here
      },
    },
  };
  </script>
  
  <style scoped>
  footer {
  margin-top: 20px;
  padding: 10px;
  background-color: #f8f9fa;
  border-top: 1px solid #ddd;
}
  </style>
  