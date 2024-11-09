<template>
    <!-- Hero section -->
    <section class="bg-teal-950 text-white h-screen flex flex-col lg:flex-row items-center px-12 lg:px-12">
        <!-- text content section -->
        <div class="max-w-7xl mx-auto flex flex-col items-center lg:items-start text-center lg:text-left lg:w-1/2 px-6 lg:px-16 mt 4">
            <!-- Heading -->
            <h1 class="text-xl md:text-3xl font-bold mb-8 mt-16">
            Create your technical drawings in just 3 clicks using ClickDraw
            </h1>
            <p class="text-md md:text-xl font-medium mb-8">
            ClickDraw, Your <strong>Drawing Copilot</strong> automates drafting process 100%
            </p>
            <p class="text-md md:text-lg font-small mb-8">
            
            </p>

            <!-- Button -->
            <div class="flex space-x-4 justify-center lg:justify-start">
            <!-- Demo Button -->
            <button @click='goToDemo' id='/demo' class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out ">
                Try the Demo
            </button>

            

            <!-- Learn More Button with opposite color scheme -->
            <button @click='goToWhatsInside' id='/whatsinside' class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out ">
                Learn More
            </button>
            </div>
            <br>
           <!-- Logo Grid Section -->
            <div class="flex justify-center">
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-12 mt-8">
                    <!-- Logo 1 -->
                    <div class="flex flex-col items-center">
                        <img src="/static/images/SolidWorks_Logo.png" alt="Software Logo 1" class="h-14 w-36 object-contain mb-0">
                        <p class="text-sm text-center italic">Integration Available</p>
                    </div>
                    
                    <!-- Logo 2 -->
                    <div class="flex flex-col items-center">
                        <img src="/static/images/PTC_Creo.png" alt="Software Logo 2" class="h-14 w-36 object-contain mb-0">
                        <p class="text-sm text-center italic">Integrating soon</p>
                    </div>
                    
                    <!-- Additional logos can be added here -->
                </div>
            </div>
           
        </div>
        

        <!-- Video Section -->
        <div class="w-full lg:w-1/2 mx-auto mt-8 lg:mt-0 relative overflow-hidden rounded-lg shadow-lg border border-gray-700">
            <div class="relative pb-[56.25%] w-full">
              <video class="absolute top-0 left-0 w-full h-full object-cover" autoplay loop muted>
                <source src="/static/videos/product_demo_version2.5.mp4" type="video/mp4">
                Your browser does not support the video tag.
              </video>
              <!-- Overlay for transparency -->
              <div class="absolute inset-0 bg-black opacity-20"></div>
            </div>
        </div>
    </section>

    <!-- Tool Leverage section  -->
    <section class="bg-gray-900 text-white py-16">
        <div class="max-w-7xl mx-auto px-6 lg:px-8">
            <!-- Section Heading -->
            <h2 class="text-xl md:text-3xl font-bold text-center mb-12">
                Are you Tired of Errors and Delays in Production Drawings?
            </h2>
    
            <!-- Feature List -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
                <!-- Feature 1 - Slide slightly from left on hover -->
                <div class="p-6 bg-gray-800 rounded-lg shadow-lg flex flex-col items-center text-center border-2 border-transparent hover:border-green-600 hover:shadow-2xl transform hover:translate-x-4 transition duration-300">
                    <div class="items-center text-center">
                        <img src="/static/images/favicon.png" alt="Icon representing QA cycle issues" class="h-12 mb-6">
                    </div>
                    <div class="items-center text-center">
                        <h3 class="text-2xl font-semibold mb-4">Endless QA Cycles?</h3>
                        <p class="text-lg text-gray-300">
                            Eliminate errors with consistent, accurate results.
                        </p>
                    </div>
                </div>
    
                <!-- Feature 2 - Slide slightly from right on hover -->
                <div class="p-6 bg-gray-800 rounded-lg shadow-lg flex flex-col items-center text-center border-2 border-transparent hover:border-green-600 hover:shadow-2xl transform hover:-translate-x-2 transition duration-300">
                    <div class="items-center text-center">
                        <img src="/static/images/favicon.png" alt="Icon representing QA cycle issues" class="h-12 mb-6">
                    </div>
                    <div class="items-center text-center">
                        <h3 class="text-2xl font-semibold mb-4">Hours Spent Drafting?</h3>
                        <p class="text-lg text-gray-300">
                            ClickDraw automates 2D drawings in seconds.
                        </p>
                    </div>
                </div>
    
                <!-- Feature 3 - Slide slightly from left on hover -->
                <div class="p-6 bg-gray-800 rounded-lg shadow-lg flex flex-col items-center text-center border-2 border-transparent hover:border-green-600 hover:shadow-2xl transform hover:translate-x-2 transition duration-300">
                    <div class="items-center text-center">
                        <img src="/static/images/favicon.png" alt="Icon representing QA cycle issues" class="h-12 mb-6">
                    </div>
                    <div class="items-center text-center">
                        <h3 class="text-2xl font-semibold mb-4">Dreading Dimensioning?</h3>
                        <p class="text-lg text-gray-300">
                            Our software handles complex designs effortlessly.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- why click draw section -->
    <section class="bg-gray-900 text-white py-16">
        <div class="max-w-7xl mx-auto px-6 lg:px-8 flex flex-col md:flex-row items-center">
            <!-- Image or Video Section -->
            <div class="w-full md:w-1/2 mb-8 md:mb-0">
                <div class="aspect-w-16 aspect-h-9">
                    <!-- Video or Image Placeholder -->
                    <img src="/static/images/clickLogoTransparent.png" alt="Top down view of walnut card tray with embedded magnets and card groove.">

                    <!-- <video controls class="w-full h-full rounded-lg shadow-lg">
                        <source src="/static/images/clickLogoTransparent.png" class="rounded-lg bg-gray-700 shadow-lg">
                        Your browser does not support the video tag.
                    </video> -->
                    <!-- If using an image instead of a video -->
                    <!-- <img src="/static/images/why-clickdraw.png" alt="Why ClickDraw" class="rounded-lg shadow-lg w-full h-auto"> -->
                </div>
            </div>

            <!-- Bullet Points Section -->
            <div class="w-full md:w-1/2 md:pl-12">
                <h2 class="text-xl md:text-3xl font-bold mb-6">Why ClickDraw?</h2>
                <ul class="list-disc pl-5 space-y-4 text-md md:text-lg">
                    <li><strong>Effortless Integration:</strong> Seamlessly integrates with your local design tools as an add-in for effortless implementation.</li>
                    <li><strong>Streamlined Workflows:</strong> Save time with user-customized templates that fit your specific needs.</li>
                    <li><strong>Quick Approvals:</strong> Submit your work for review and approval without time-consuming manual cross-checking.</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Technical Specifications section -->
    <section class="bg-gray-900 text-white py-16">
        <div id="whatsinside" class="max-w-7xl mx-auto px-6 lg:px-8">
            <div class="mx-auto grid max-w-2xl grid-cols-1 items-center gap-x-8 gap-y-16 px-4 py-24 sm:px-6 sm:py-32 lg:max-w-7xl lg:grid-cols-2 lg:px-8">
                <!-- Text and Specifications List -->
                <div>
                    <h2 class="text-xl md:text-3xl font-bold mb-6">What's Inside ClickDraw?</h2>
                    <p class="mt-4 text-lg text-gray-300">
                        
                    </p>

                    <dl class="mt-16 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 sm:gap-y-16 lg:gap-x-8">
                        <div class="border-t border-gray-700 pt-4">
                            <dt class="font-medium text-white">Dimension Definer</dt>
                            <dd class="mt-2 text-sm text-gray-300">Native-developed algorithms for effortless Dimension definition.</dd>
                        </div>
                        <div class="border-t border-gray-700 pt-4">
                            <dt class="font-medium text-white">Views Maker</dt>
                            <dd class="mt-2 text-sm text-gray-300">Smart dimensioning, minimalist views - clarity redefined.</dd>
                        </div>
                        <div class="border-t border-gray-700 pt-4">
                            <dt class="font-medium text-white">Drawing Copilot</dt>
                            <dd class="mt-2 text-sm text-gray-300">Let our plugin create drawings alongside your design, automatically.</dd>
                        </div>      
                    </dl>
                </div>

                <!-- Image Gallery -->
                <div class="grid grid-cols-2 grid-rows-2 gap-4 sm:gap-6 lg:gap-8">
                    
                    <img src="/static/images/view_selector_02.png" 
                         alt="Top down view of walnut card tray with embedded magnets and card groove." 
                         class="rounded-lg bg-gray-700 shadow-lg transform hover:scale-110 transition duration-300 ease-in-out">
                
                    <img src="/static/images/view_selector_02.png" 
                         alt="Top down view of walnut card tray with embedded magnets and card groove." 
                         class="rounded-lg bg-gray-700 shadow-lg transform hover:scale-110 transition duration-300 ease-in-out">
                
                    <img src="/static/images/view_selector_02.png" 
                         alt="Top down view of walnut card tray with embedded magnets and card groove." 
                         class="rounded-lg bg-gray-700 shadow-lg transform hover:scale-110 transition duration-300 ease-in-out">
                    
                    <img src="/static/images/view_selector_02.png" 
                         alt="Top down view of walnut card tray with embedded magnets and card groove." 
                         class="rounded-lg bg-gray-700 shadow-lg transform hover:scale-110 transition duration-300 ease-in-out">
                </div>
            </div>
        </div>
    </section>

    <!-- demo video section -->

    

    <section class="bg-gray-900 text-white">
        <div id="demo" class="w-full px-0 lg:px-0"> <!-- Ensure no padding here -->
            <h2 class="text-xl md:text-3xl font-bold text-center mb-8">Watch Our Demo</h2>
            <p class="text-md md:text-xl text-center mb-8">See ClickDraw in action and discover how it can simplify your drawing process.</p>
            
            <!-- Full width container for the video -->
            <div class="flex justify-center w-full">
                <div class="relative w-full" style="padding-top: 56.25%;"> <!-- 16:9 Aspect Ratio -->
                    <iframe 
                        src="https://www.youtube.com/embed/VIDEO_ID" 
                        title="YouTube video player" 
                        class="absolute top-0 left-0 w-full h-full shadow-md" 
                        frameborder="0" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen>
                    </iframe>
                </div>
            </div>
        </div>
    </section>


    <!-- FAQ Section -->
    <section class="bg-gray-900 text-white py-16">
        <div class="max-w-4xl mx-auto px-6 lg:px-8">
        <!-- Section Heading -->
        <h2 class="text-xl md:text-3xl font-bold text-center mb-12">
            Frequently Asked Questions
        </h2>

        <!-- FAQ Items -->
        <div class="space-y-4">
            <!-- Question 1 - Open by default -->
            <div class="bg-gray-800 p-6 rounded-lg">
            <button @click="toggleFaq(1)" class="w-full text-left flex justify-between items-center">
                <span class="text-xl font-semibold">What is ClickDraw?</span>
                <svg :class="{'rotate-180': activeFaq === 1}" class="w-6 h-6 transition-transform" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M5.293 9.293a1 1 0 011.414 0L10 12.586l3.293-3.293a1 1 0 011.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                </svg>
            </button>
            <div v-show="activeFaq === 1" class="mt-4 text-gray-300">
                <p>ClickDraw is a drawing automation tool developed to generate technical drawings with just 3 clicks effort. It streamlines the process, reducing errors and speeding up production.</p>
            </div>
            </div>

            <!-- Question 2 -->
            <div class="bg-gray-800 p-6 rounded-lg">
            <button @click="toggleFaq(2)" class="w-full text-left flex justify-between items-center">
                <span class="text-xl font-semibold">How does ClickDraw work?</span>
                <svg :class="{'rotate-180': activeFaq === 2}" class="w-6 h-6 transition-transform" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M5.293 9.293a1 1 0 011.414 0L10 12.586l3.293-3.293a1 1 0 011.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                </svg>
            </button>
            <div v-show="activeFaq === 2" class="mt-4 text-gray-300">
                <p>ClickDraw automates the creation of 2D technical drawings from CAD data. It identifies key design elements, applies predefined templates, and generates drawings with annotations and dimensions, all in just a few clicks.</p>
            </div>
            </div>

            <!-- Question 3 -->
            <div class="bg-gray-800 p-6 rounded-lg">
            <button @click="toggleFaq(3)" class="w-full text-left flex justify-between items-center">
                <span class="text-xl font-semibold">Is there a free trial available?</span>
                <svg :class="{'rotate-180': activeFaq === 3}" class="w-6 h-6 transition-transform" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M5.293 9.293a1 1 0 011.414 0L10 12.586l3.293-3.293a1 1 0 011.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                </svg>
            </button>
            <div v-show="activeFaq === 3" class="mt-4 text-gray-300">
                <p>Yes, you can sign up for a free trial to explore the basic features of ClickDraw. The trial allows you to generate a limited number of technical drawings.</p>
            </div>
            </div>
        </div>
        </div>
    </section>

    <!-- Pricing section -->
    <section class="bg-gray-900 text-white py-16">
    <div class="max-w-7xl mx-auto px-6 lg:px-8">
        <!-- Section Heading -->
        <h2 class="text-xl md:text-3xl font-bold text-center mb-12">
        Choose Your Plan
        </h2>
        <div class="flex justify-center">
            <p class="text-lg md:text-xl font-small mb-8 text-center max-w-2xl lg:max-w-3xl">
            We focus on markets where technology, innovation, and capital can unlock long-term value and drive economic growth.
            </p>
        </div>


        <!-- Pricing Cards -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Free Trial Plan -->
        <div class="bg-gray-800 p-8 rounded-lg shadow-lg text-center transform hover:scale-110 transition duration-300 ease-in-out">
            <h3 class="text-2xl font-semibold mb-6">Freemium</h3>
            <div class="text-5xl font-bold mb-4 flex justify-center items-center">
            <span class="text-3xl mr-1">₹</span> 0 <span class="text-xl mr-1"> &nbsp / year</span>
            </div>
            <p class="text-gray-300 mb-8">
            Get started for free and explore the basic features.
            </p>
            <!-- Bullet points -->
            <ul class="mb-8 text-left">
            <li class="flex items-center mb-2">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Access to basic features
            </li>
            <li class="flex items-center mb-2">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Can generate 300 drawings / year
            </li>
            <li class="flex items-center">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Access to customer support
            </li>
            </ul>
            <NuxtLink to="/contact" class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out">
            Start Free Trial
            </NuxtLink>
        </div>

        <!-- Starter Pack Plan -->
        <div class="bg-gray-800 p-8 rounded-lg shadow-lg text-center transform hover:scale-110 transition duration-300 ease-in-out">
            <h3 class="text-2xl font-semibold mb-6">Basic</h3>
            <div class="text-5xl font-bold mb-4 flex justify-center items-center">
            <span class="text-3xl mr-1">₹</span>50000 <span class="text-xl mr-1">&nbsp / year</span>
            </div>
            <p class="text-gray-300 mb-8">
            Access more features and increase productivity.
            </p>
            <!-- Bullet points -->
            <ul class="mb-8 text-left">
            <li class="flex items-center mb-2">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Access to all features
            </li>
            <li class="flex items-center mb-2">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Can generate 1000 drawings / year
            </li>
            <li class="flex items-center">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Priority Support
            </li>
            </ul>
            <NuxtLink to="/contact" class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out">
            Start Basic Plan
            </NuxtLink>
        </div>

        <!-- Premium Plan -->
        <div class="bg-gray-800 p-8 rounded-lg shadow-lg text-center transform hover:scale-110 transition duration-300 ease-in-out">
            <h3 class="text-2xl font-semibold mb-6">Premium</h3>
            <div class="text-5xl font-bold mb-4 flex justify-center items-center">
            <span class="text-3xl mr-1">₹</span>10 <span class="text-xl mr-1"> &nbsp lakhs / year</span>
            </div>
            <p class="text-gray-300 mb-8">
            Unlock all features for the ultimate experience.
            </p>
            <!-- Bullet points -->
            <ul class="mb-8 text-left">
            <li class="flex items-center mb-2">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Access to premium features
            </li>
            <li class="flex items-center mb-2">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                Unlimited storage
            </li>
            <li class="flex items-center">
                <svg class="w-5 h-5 text-green-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 00-1.414-1.414L9 10.172l-2.293-2.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l7-7z" clip-rule="evenodd" />
                </svg>
                24/7 VIP Support
            </li>
            </ul>
            <NuxtLink to="/contact" class="bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-6 rounded-full transition duration-300 ease-in-out">
            Start Premium Plan
            </NuxtLink>
        </div>
        </div>
    </div>
    </section>

    <!-- Client base section -->
    <section class="bg-gray-900 text-white py-16">
        <div class="max-w-7xl mx-auto px-6 lg:px-8">
            <h2 class="text-xl md:text-3xl font-bold text-center mb-8">Our Clients</h2>
            <p class="text-md md:text-xl text-center mb-12">
            Trusted by leading brands and innovators.
            </p>
            <div class="flex justify-center gap-8">
                
            </div>
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8 ">
                <!-- Client 1 -->
                <div class="flex items-center justify-center bg-white p-4 rounded-lg">
                    <a href="https://www.modulushousing.com/" target="_blank" rel="noopener noreferrer">
                        <img src="/static/images/customerlogo/modulus housing.webp" alt="Client 1" class="h-12 md:h-16 mx-auto" />
                    </a>
                </div>
                <!-- Client 2 -->
                <div class="flex items-center justify-center bg-white p-4 rounded-lg">
                    <a href="https://www.linkedin.com/company/cbeev?originalSubdomain=in" target="_blank" rel="noopener noreferrer">
                        <img src="/static/images/customerlogo/cbeev.png" alt="Client 1" class="h-12 md:h-16 mx-auto" />
                    </a>
                </div>
                <!-- Client 3 -->
                <div class="flex items-center justify-center bg-white p-4 rounded-lg">
                    <img src="/static/images/favicon.png" alt="Client 3" class="h-12 md:h-16 mx-auto" />
                </div>
                <!-- Client 3 -->
                <div class="flex items-center justify-center bg-white p-4 rounded-lg">
                    <img src="/static/images/favicon.png" alt="Client 3" class="h-12 md:h-16 mx-auto" />
                </div>
            <!-- Add more client logos as needed -->
            </div>
        </div>
    </section>

    <!-- Testimonial section -->
    <section class="bg-gray-900 text-white py-16">
        <div class="max-w-3xl mx-auto px-6 lg:px-8">
            <h2 class="text-xl md:text-3xl font-bold text-center mb-8">What Our Clients Say</h2>
            <div class="bg-gray-800 rounded-lg shadow-md p-8">
            <div class="flex justify-center mb-4">
                <svg class="w-8 h-8 text-green-500" fill="currentColor" viewBox="0 0 20 20">
                <path d="M10 3a7 7 0 100 14 7 7 0 000-14zm0 12a5 5 0 110-10 5 5 0 010 10z" />
                </svg>
            </div>
            <p class="text-center italic">"{{ testimonials[currentTestimonial].quote }}"</p>
            <div class="mt-4 text-center">
                <p class="font-bold">{{ testimonials[currentTestimonial].name }}</p>
                <p class="text-gray-400">{{ testimonials[currentTestimonial].company }}</p>
            </div>
            <div class="flex justify-between mt-6">
                <button @click="prevTestimonial" class="bg-gray-700 p-2 rounded hover:bg-gray-600">Previous</button>
                <button @click="nextTestimonial" class="bg-gray-700 p-2 rounded hover:bg-gray-600">Next</button>
            </div>
            </div>
        </div>
    </section>

    <!-- Contact us section -->
    <section id="contact" class="bg-teal-950 text-white py-16">
        <div class="container mx-auto px-6 lg:px-8">
            <div class="section-title text-center mb-12">
                <h2 class="text-xl md:text-3xl font-bold">Contact Us</h2>
                <p class="text-md md:text-lg mt-4">We're here to help you! Reach out to us anytime.</p>
            </div>
            <div class="flex flex-col lg:flex-row lg:space-x-10">
                <!-- Map Section -->
                <div class="lg:w-1/2 mb-8 lg:mb-0 px-5 lg:px-10">
                <iframe
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3887.6996859578626!2d80.24036047489335!3d12.991049987326111!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3a5267c744de252b%3A0x8475b6b43cdae847!2sFUTAUCON%20TEK%20PVT%20LTD!5e0!3m2!1sen!2sin!4v1713249388676!5m2!1sen!2sin"
                    frameborder="0"
                    style="border:0; height: 400px; width: 100%;"
                    allowfullscreen=""
                    loading="lazy">
                </iframe>
                </div>
                <!-- Contact Info Section -->
                <div class="lg:w-1/2 px-5 lg:px-10">
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
                        <div class="flex flex-col md:flex-row justify-between gap-8">
                            <!-- Info Box for Email -->
                            <div class="info-box p-6 bg-gray-800 shadow-lg rounded-lg flex items-start w-full">
                                <i class="fas fa-envelope text-green-500 text-3xl mr-4"></i>
                                <div>
                                <h3 class="text-lg font-semibold">Email Us</h3>
                                <p>vijay@futaucon.com</p>
                                </div>
                            </div>

                            <!-- Info Box for Phone -->
                            <div class="info-box p-6 bg-gray-800 shadow-lg rounded-lg flex items-start w-full">
                                <i class="fas fa-phone-alt text-green-500 text-3xl mr-4"></i>
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
    </section>

  </template>




<script>
export default {
  name: "Index",
  data() {
    return {
      activeFaq: 1, // Default open FAQ
      currentTestimonial: 0, // Index for the current testimonial
      testimonials: [
        {
          quote: "ClickDraw has transformed our drawing process!",
          name: "Arun",
          company: "Yali Mobility",
        },
        {
          quote: "A game-changer for our engineering team!",
          name: "Sriram",
          company: "Modulus Housing",
        },
        {
          quote: "Fast, efficient, and reliable. Highly recommend!",
          name: "kishore",
          company: "Caterpillar",
        },
      ],
    };
  },
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
    goToDemo() {
      const demoSection = document.getElementById('demo'); // Get the section with id 'demo'
      if (demoSection) {
        demoSection.scrollIntoView({ behavior: 'smooth' }); // Scroll to the section smoothly
      } else {
        console.warn("Section with id 'demo' not found");
      }
    },
    goToWhatsInside() {
        const demoSection = document.getElementById('whatsinside'); // Get the section with id 'demo'
        if (demoSection) {
          demoSection.scrollIntoView({ behavior: 'smooth' }); // Scroll to the section smoothly
        } else {
          console.warn("Section with id 'WhatsInside' not found");
        }
      },
  },
  mounted() {
    // Auto-slide testimonials every 5 seconds
    setInterval(this.nextTestimonial, 5000);
  },
};
</script>