<template>
  <div class="image-container">
    <img :src="imageSrc" class="landing-image">
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageSrc: require('@/images/417566036_1425595901716331_2388011869341318955_n-removebg-preview.png')
    }
  }
}
</script>

<style>

.image-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; 
  width: 100vw; 
}


.landing-image {
  max-width: 100%;
  max-height: 100vh; /* Adjust the height to fit the viewport */
  object-fit: cover; /* Cover the container without losing aspect ratio */
}
</style>