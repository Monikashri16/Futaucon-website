<template>
  <div class="bg-gray-900 min-h-screen flex flex-col md:flex-row text-white">
    <!-- Left Side: Contact Details -->
    <div class="md:w-1/2 p-6 flex flex-col justify-center items-start">
      <h2 class="text-2xl font-bold mb-4">Contact Us</h2>
      <p class="mb-2">Phone: +91 90803 27984</p>
      <p class="mb-2">Email: vijay@futaucon.com</p>
      <p class="mb-2">Address: 1st floor, E Block, IITM Research Park<br> Tharamani, Chennai-600113</p>
      <div class="mt-6">
        <h3 class="text-xl font-semibold mb-2">Follow Us</h3>
        <div class="flex space-x-4">
          <a href="#" class="text-blue-400 hover:text-blue-600">Facebook</a>
          <a href="#" class="text-blue-400 hover:text-blue-600">Twitter</a>
          <a href="#" class="text-blue-400 hover:text-blue-600">LinkedIn</a>
        </div>
      </div>
    </div>

    <!-- Right Side: Form -->
    <div class="md:w-1/2 p-6 bg-gray-800 flex items-center justify-center">
      <form class="w-full max-w-lg bg-gray-700 p-6 rounded-lg shadow-lg">
        <h2 class="text-2xl font-bold mb-4">Get in Touch</h2>
        <div class="mb-4">
          <label class="block text-sm font-medium mb-1" for="name">Name</label>
          <input
            id="name"
            type="text"
            class="w-full p-3 border rounded bg-gray-800 text-white focus:outline-none focus:ring focus:ring-blue-500"
            placeholder="Your Name"
          />
        </div>
        <div class="mb-4">
          <label class="block text-sm font-medium mb-1" for="email">Email</label>
          <input
            id="email"
            type="email"
            class="w-full p-3 border rounded bg-gray-800 text-white focus:outline-none focus:ring focus:ring-blue-500"
            placeholder="Your Email"
          />
        </div>
        <div class="mb-4">
          <label class="block text-sm font-medium mb-1" for="company name">Company Name</label>
          <input
            id="plan"
            type="text"
            class="w-full p-3 border rounded bg-gray-800 text-white focus:outline-none focus:ring focus:ring-blue-500"
            placeholder="Your Company Name"
          />
        </div>
        <div class="mb-4">
          <label class="block text-sm font-medium mb-1" for="plan">Which Plan?</label>
          <div class="flex flex-col space-y-2 mt-2">
            <label class="inline-flex items-center">
              <input
                type="radio"
                name="plan"
                value="freemium"
                class="text-blue-500 focus:ring focus:ring-blue-500"
              />
              <span class="ml-2">Freemium</span>
            </label>
            <label class="inline-flex items-center">
              <input
                type="radio"
                name="plan"
                value="basic"
                class="text-blue-500 focus:ring focus:ring-blue-500"
              />
              <span class="ml-2">Basic</span>
            </label>
            <label class="inline-flex items-center">
              <input
                type="radio"
                name="plan"
                value="premium"
                class="text-blue-500 focus:ring focus:ring-blue-500"
              />
              <span class="ml-2">Premium</span>
            </label>
          </div>
        </div>
        <div class="mb-4">
          <label class="block text-sm font-medium mb-1" for="message">Message</label>
          <textarea
            id="message"
            class="w-full p-3 border rounded bg-gray-800 text-white focus:outline-none focus:ring focus:ring-blue-500"
            rows="4"
            placeholder="I am interested in this plan"
          ></textarea>
        </div>
        <button
          type="submit"
          class="w-full bg-blue-600 hover:bg-blue-700 text-white font-semibold py-3 rounded-lg focus:outline-none focus:ring focus:ring-blue-500"
        >
          Send Message
        </button>
      </form>
    </div>   
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