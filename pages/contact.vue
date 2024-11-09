<template>
  <div class="bg-gray-900 h-screen">   
  </div>
</template>

<script>
export default {
name: "Contact",
methods: {
  toggleFaq(id) {
    this.activeFaq = this.activeFaq === id ? null : id;
  },
  nextTestimonial() {
    this.currentTestimonial = (this.currentTestimonial + 1) % this.testimonials.length;
  },
  prevTestimonial() {
    this.currentTestimonial = (this.currentTestimonial - 1 + this.testimonials.length) % this.testimonials.length;
  },
  
},

};
</script>

<style scoped>
/* You can add custom styling here if needed */
</style>