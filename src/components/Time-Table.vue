<template>
  <div class="time-table-container">
    <v-card class="class-card mb-4">
      <v-card-title>BJJ Class - Tuesday</v-card-title>
      <v-card-text>7:30 PM - 8:30 PM</v-card-text>
    </v-card>
    <v-card class="class-card">
      <v-card-title>BJJ Class - Saturday</v-card-title>
      <v-card-text>8:00 AM - 9:00 AM</v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
};
</script>

<style scoped>
.time-table-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  background: #15202b;
}

.class-card {
  max-width: 80%; 
  background-color: #ffffff; 
  color: #000000; 
  box-shadow: 0 4px 8px rgba(0,0,0,0.2); 
}

.mb-4 {
  margin-bottom: 16px; 
}
</style>