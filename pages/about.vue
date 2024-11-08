<template>
  <div class="bg-gray-900 h-screen">
    
    <!-- Image Section -->
    <section>
      <img 
        src="https://damassets.autodesk.net/content/dam/autodesk/www/solutions/generative-design/fy22/images/drafting-software-programs/making-blueprint-drawings-thumb-788x444.jpg" 
        alt="Descriptive Alt Text" 
        class="w-full h-40 object-cover"
      >
      <div class="absolute inset-0 flex items-center justify-center bg-opacity-50 transition-opacity duration-300 mb-5">
        <p class="text-green-500 text-2xl font-bold">ABOUT</p>
      </div>
    </section>
    
    
  </div>
  <div>
    <section class>
      <div class="mx-auto grid grid-cols-2">
        <!-- Each Image in the Window Pane -->
        <div class="relative group overflow-hidden">
          <img src="https://img.freepik.com/premium-photo/hand-sketching-blueprint-with-pencil-dimly-lit-room_1317208-2238.jpg?semt=ais_hybrid" alt="Photo 1" class="w-full h-full object-cover transition-transform duration-300">
          <div class="absolute inset-0 flex items-center justify-center bg-opacity-50 opacity-50 group-hover:opacity-100 transition-opacity duration-300 group-hover:-translate-y-2">
            <p class="text-white text-lg font-semibold">Image 1 Caption</p>
          </div>
        </div>
        <div class="relative group overflow-hidden">
          <img src="https://img.freepik.com/premium-photo/hand-sketching-blueprint-with-pencil-dimly-lit-room_1317208-2238.jpg?semt=ais_hybrid" alt="Photo 2" class="w-full h-full object-cover transition-transform duration-300 ">
          <div class="absolute inset-0 flex items-center justify-center bg-opacity-50 opacity-50 group-hover:opacity-100 transition-opacity duration-300 group-hover:-translate-y-2">
            <p class="text-white text-lg font-semibold">Image 2 Caption</p>
          </div>
        </div>
        <div class="relative group overflow-hidden">
          <img src="https://img.freepik.com/premium-photo/cropped-shot-engineers-architects-are-helping-design-construction_36897-59819.jpg?semt=ais_hybrid" alt="Photo 3" class="w-full h-full object-cover transition-transform duration-300">
          <div class="absolute inset-0 flex items-center justify-center bg-opacity-50 opacity-50 group-hover:opacity-100 transition-opacity duration-300 group-hover:-translate-y-2">
            <p class="text-white text-lg font-semibold">Image 3 Caption</p>
          </div>
        </div>
        <div class="relative group overflow-hidden">
          <img src="https://img.freepik.com/premium-photo/cropped-shot-engineers-architects-are-helping-design-construction_36897-59819.jpg?semt=ais_hybrid" alt="Photo 4" class="w-full h-full object-cover transition-transform duration-300">
          <div class="absolute inset-0 flex items-center justify-center bg-opacity-50 opacity-50 group-hover:opacity-100 transition-opacity duration-300 group-hover:-translate-y-2">
            <p class="text-white text-lg font-semibold">Image 4 Caption</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
name: "About",
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