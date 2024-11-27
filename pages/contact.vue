<template>
  <div class="bg-gray-900 min-h-screen flex flex-col-reverse md:flex-row text-white">
    <!-- Left Side: Form -->
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

    <!-- Right Side: Contact Details -->
    <div class="md:w-1/2 p-6 flex flex-col justify-center items-start">
      <div class="lg:w-4/5 px-5 lg:px-10">
        <div class="space-y-8">
            <!-- Info Box for Address -->
            <div class="info-box p-6 bg-gray-800 shadow-lg rounded-lg flex items-start">
            <i class="fas fa-map-marker-alt text-green-500 text-3xl mr-4"></i>
                <div>
                    <h3 class="text-lg font-semibold">Visit Us!</h3>
                    <p>1st floor, E Block, IITM Research Park<br> Tharamani, Chennai-600113</p>
                </div>
            </div>

            <!-- Flex container for Email and Phone -->
            <div class="flex flex-col md:flex-row justify-between gap-1">
                <!-- Info Box for Email -->
                <div class="info-box p-6 bg-gray-800 shadow-lg rounded-lg flex items-start w-full">
                    <i class="fas fa-envelope text-green-500 text-3xl mr-1"></i>
                    <div>
                    <h3 class="text-lg font-semibold">Email Us</h3>
                    <p>vijay@futaucon.com</p>
                    </div>
                </div>

                <!-- Info Box for Phone -->
                <div class="info-box p-6 bg-gray-800 shadow-lg rounded-lg flex items-start w-full">
                    <i class="fas fa-phone-alt text-green-500 text-3xl mr-1"></i>
                    <div>
                    <h3 class="text-lg font-semibold">Call Us</h3>
                    <p>+91 90803 27984</p>
                    </div>
                </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactPage",
  data() {
    return {
      tabBarName: "Contact Us", // Default tab name
    };
  },
  watch: {
    // Watch for changes in tabBarName and update the browser's tab title
    tabBarName(newVal) {
      document.title = `${newVal} | Futaucon`; // Update browser tab title dynamically
    },
  },
  methods: {
    // Update the tabBarName (can be expanded for dynamic tabs)
    updateTabName(name) {
      this.tabBarName = name;
    },
  },
  mounted() {
    // Initialize the browser tab title
    document.title = `${this.tabBarName} | Futaucon`;
  },
};
</script>

<style scoped>
/* You can add custom styling here */
</style>

