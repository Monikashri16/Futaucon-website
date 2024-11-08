<template>
    <header>
    <nav class="border-b border-gray-700 bg-stone-700 text-white"> <!-- Update background color -->
      
      <div class="flex justify-between items-center max-w-7xl mx-auto px-2 py-4">
        <!-- Logo -->
        <div class="flex-shrink-0">
          <NuxtLink to="/">
            <img src="/static/images/logo.png" alt="Company Logo" class="h-8 w-auto m-2">
          </NuxtLink>
        </div>

        <ul class="flex justify-center space-x-8 mr-4">
          <!-- Top-level Navigation Items -->
          <li class="hover:text-teal-950"> <!-- Change hover text color -->
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li class="hover:text-teal-950">
            <NuxtLink to="/about">About</NuxtLink>
          </li>
        </ul>
        
      
      </div>
    </nav>
  </header>
</template>
  
    <script>
    export default {
    data() {
      return {
        activeDropdown: null, // State to track the active dropdown
      };
    },
    methods: {
  // Generic method to toggle dropdowns
  toggleDropdown(menu) {
      // Check if the menu is already active
      if (this.activeDropdown === menu) {
      this.activeDropdown = null; // Close dropdown if it's already open
      this.removeClickOutsideListener(); // Remove click listener
      } else {
      this.activeDropdown = menu; // Open the clicked dropdown
      this.$nextTick(() => this.addClickOutsideListener()); // Add click listener
      }
  },
  // Add a listener to detect clicks outside the dropdown
  addClickOutsideListener() {
      document.addEventListener('click', this.handleClickOutside);
  },
  // Remove the click outside listener
  removeClickOutsideListener() {
      document.removeEventListener('click', this.handleClickOutside);
  },
  // Handler to close the dropdown if clicked outside
  handleClickOutside(event) {
      const dropdownElement = this.$el.querySelector('.relative'); // Target the dropdown element
      if (!dropdownElement.contains(event.target)) {
      this.activeDropdown = null; // Close dropdown
      this.removeClickOutsideListener(); // Remove listener
      }
  },
    },
    beforeDestroy() {
      // Clean up the event listener when the component is destroyed
      this.removeClickOutsideListener();
    }
  };
    </script>
    
  
  
    <style scoped>
    /* Add additional custom styles here if needed */
    </style>