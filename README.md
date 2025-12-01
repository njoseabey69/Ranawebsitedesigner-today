<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Rana - Creative Web Designer, Developer & computer solutions</title>
    <script src="https://cdn.tailwindcss.com/3.4.16"></script>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            colors: { primary: "#4F46E5", secondary: "#10B981" },
            borderRadius: {
              none: "0px",
              sm: "4px",
              DEFAULT: "8px",
              md: "12px",
              lg: "16px",
              xl: "20px",
              "2xl": "24px",
              "3xl": "32px",
              full: "9999px",
              button: "8px",
            },
          },
        },
      };
    </script>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap"
      rel="stylesheet"
    />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap"
      rel="stylesheet"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/remixicon/4.6.0/remixicon.min.css"
    />
    <style>
      :where([class^="ri-"])::before { content: "\f3c2"; }
      body {
      font-family: 'Inter', sans-serif;
      scroll-behavior: smooth;
      }
      .hero-bg {
      background-position: center;
      background-size: cover;
      background-repeat: no-repeat;
      }
      .portfolio-item {
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      }
      .portfolio-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      }
      .portfolio-overlay {
      opacity: 0;
      transition: opacity 0.3s ease;
      }
      .portfolio-item:hover .portfolio-overlay {
      opacity: 1;
      }
      .skill-bar {
      height: 8px;
      border-radius: 4px;
      background-color: #e5e7eb;
      overflow: hidden;
      }
      .skill-progress {
      height: 100%;
      border-radius: 4px;
      }
      input:focus, textarea:focus {
      outline: none;
      border-color: #4F46E5;
      }
      .nav-link {
      position: relative;
      }
      .nav-link::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -2px;
      left: 0;
      background-color: #4F46E5;
      transition: width 0.3s ease;
      }
      .nav-link:hover::after, .nav-link.active::after {
      width: 100%;
      }
      .custom-checkbox {
      appearance: none;
      -webkit-appearance: none;
      width: 20px;
      height: 20px;
      border: 2px solid #d1d5db;
      border-radius: 4px;
      outline: none;
      cursor: pointer;
      position: relative;
      }
      .custom-checkbox:checked {
      background-color: #4F46E5;
      border-color: #4F46E5;
      }
      .custom-checkbox:checked::after {
      content: '';
      position: absolute;
      top: 3px;
      left: 6px;
      width: 6px;
      height: 10px;
      border: solid white;
      border-width: 0 2px 2px 0;
      transform: rotate(45deg);
      }
    </style>
  </head>
  <body class="bg-white">
    <!-- Header Section -->
    <header
      class="fixed top-0 left-0 right-0 bg-white shadow-sm z-50 transition-all duration-300"
    >
      <div
        class="container mx-auto px-6 py-4 flex items-center justify-between"
      ><img src="\Users\ABEY\Downloads\new web log.png" alt="RANA WEBSITE DESIGNERS" width="100" height="100">
     
        <a href="#" class="text-2xl font-['Pacifico'] text-primary">RANA WEBSITE DESIGNERS</a>
        <nav class="hidden md:flex items-center space-x-8">
          <a
            href="#home"
            class="nav-link active text-gray-800 hover:text-primary transition-colors"
            >Home</a
          >
          <a
            href="#portfolio"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Portfolio</a
          >
          <a
            href="#services"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Services</a
          >
          <a
            href="#about"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >About</a
          >
          <a
            href="#contact"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Contact</a
          >
        </nav>
        <a
          href="#contact"
          class="hidden md:block bg-primary text-white px-5 py-2.5 !rounded-button font-medium hover:bg-primary/90 transition-colors whitespace-nowrap"
          >Hire Me</a
        >
        <button
          id="mobile-menu-button"
          class="md:hidden w-10 h-10 flex items-center justify-center text-gray-700"
        >
          <i class="ri-menu-line ri-lg"></i>
        </button>
      </div>
      <!-- Mobile Menu -->
      <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
        <div class="container mx-auto px-6 py-4 flex flex-col space-y-4">
          <a
            href="#home"
            class="text-gray-800 hover:text-primary py-2 transition-colors"
            >Home</a
          >
          <a
            href="#portfolio"
            class="text-gray-800 hover:text-primary py-2 transition-colors"
            >Portfolio</a
          >
          <a
            href="#services"
            class="text-gray-800 hover:text-primary py-2 transition-colors"
            >Services</a
          >
          <a
            href="#about"
            class="text-gray-800 hover:text-primary py-2 transition-colors"
            >About</a
          >
          <a
            href="#contact"
            class="text-gray-800 hover:text-primary py-2 transition-colors"
            >Contact</a
          >
          <a
            href="#contact"
            class="bg-primary text-white px-5 py-2.5 !rounded-button font-medium hover:bg-primary/90 transition-colors text-center whitespace-nowrap"
            >Hire Me</a
          >
        </div>
      </div>
    </header>
    <!-- Hero Section -->
    <section
     id="home"
      class="pt-24 hero-bg relative"
      style="background-image: url('https://readdy.ai/api/search-image?query=modern%20minimalist%20workspace%20with%20computer%2C%20design%20elements%2C%20creative%20atmosphere%2C%20soft%20lighting%2C%20professional%20environment%2C%20clean%20desk%20setup%2C%20web%20design%20elements%2C%20digital%20art%20tools%2C%20neutral%20color%20palette%2C%20inspirational%20workspace&width=1920&height=1080&seq=1&orientation=landscape')"
    >
      <div
        class="absolute inset-0 bg-gradient-to-r from-white via-white/90 to-transparent"
      ></div>
      <div class="container mx-auto px-6 py-20 md:py-32 relative">
        <div class="max-w-2xl">
          <h1
            class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-6"
          >
            Creative Web Designer, Developer & Computer slutions
          </h1>
          <p class="text-xl md:text-2xl text-gray-700 mb-8">
            Crafting Digital Experiences That Stand Out
          </p>
          <div class="flex flex-wrap gap-4">
            <a
              href="#portfolio"
              class="bg-primary text-white px-6 py-3 !rounded-button font-medium hover:bg-primary/90 transition-colors whitespace-nowrap"
            >
              View Portfolio
            </a>
            <a
              href="#contact"
              class="bg-white text-primary border-2 border-primary px-6 py-3 !rounded-button font-medium hover:bg-gray-50 transition-colors whitespace-nowrap"
            >
              Let's Talk
            </a>
          </div>
        </div>
      </div>
      <div class="absolute bottom-0 left-0 right-0 flex justify-center">
        <a
          href="#portfolio"
          class="w-10 h-10 bg-white rounded-full shadow-md flex items-center justify-center mb-8 animate-bounce"
        >
          <i class="ri-arrow-down-line text-primary"></i>
        </a>
      </div>
    </section>
    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-gray-50">
      <div class="container mx-auto px-6">
        <div class="text-center mb-12">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
            My Portfolio
          </h2>
          <p class="text-gray-600 max-w-2xl mx-auto">
            Explore my recent projects and discover how I bring ideas to life
            through thoughtful design and development.
          </p>
        </div>
        <div class="flex justify-center mb-10">
          <div class="inline-flex bg-white rounded-full p-1 shadow-sm">
            <button
              class="portfolio-filter active px-4 py-2 !rounded-full text-sm font-medium bg-primary text-white whitespace-nowrap"
            >
              All Work
            </button>
            <button
              class="portfolio-filter px-4 py-2 !rounded-full text-sm font-medium text-gray-700 hover:text-primary whitespace-nowrap"
            >
              Web Design
            </button>
            <button
              class="portfolio-filter px-4 py-2 !rounded-full text-sm font-medium text-gray-700 hover:text-primary whitespace-nowrap"
            >
              UI/UX
            </button>
            <button
              class="portfolio-filter px-4 py-2 !rounded-full text-sm font-medium text-gray-700 hover:text-primary whitespace-nowrap"
            >
              Development
            </button>
          </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Portfolio Item 1 -->
          <div
            class="portfolio-item bg-white rounded-lg overflow-hidden shadow-sm"
          >
            <div class="relative h-64">
              <img
                src="https://readdy.ai/api/search-image?query=modern%20e-commerce%20website%20design%20with%20clean%20layout%2C%20product%20showcase%2C%20minimalist%20interface%2C%20professional%20web%20design%2C%20online%20store%20homepage%20with%20elegant%20typography%2C%20shopping%20cart%20functionality%2C%20responsive%20design%20elements%2C%20white%20background%20with%20accent%20colors&width=600&height=400&seq=2&orientation=landscape"
                alt="E-commerce Website"
                class="w-full h-full object-cover object-top"
              />
              <div
                class="portfolio-overlay absolute inset-0 bg-primary/80 flex items-center justify-center p-6"
              >
                <div class="text-center text-white">
                  <h3 class="text-xl font-semibold mb-2">
                    Luxe Fashion E-commerce
                  </h3>
                  <p class="mb-4">
                    A premium online shopping experience with seamless checkout
                    and personalized recommendations.
                  </p>
                  <a
                    href="#"
                    class="inline-flex items-center text-white border-b border-white pb-1 hover:pb-2 transition-all"
                  >
                    View Details <i class="ri-arrow-right-line ml-1"></i>
                  </a>
                </div>
              </div>
            </div>
            <div class="p-6">
              <h3 class="text-lg font-semibold text-gray-900 mb-1">
                Luxe Fashion E-commerce
              </h3>
              <p class="text-gray-600 text-sm mb-3">Web Design and maintainance, Development</p>
              <a
                href="#"
                class="text-primary font-medium inline-flex items-center view-project-btn"
                data-project="Luxe Fashion E-commerce"
              >
                View Project <i class="ri-arrow-right-line ml-1"></i>
              </a>
            </div>
          </div>
          <!-- Portfolio Item 2 -->
          <div
            class="portfolio-item bg-white rounded-lg overflow-hidden shadow-sm"
          >
            <div class="relative h-64">
              <img
                src="https://readdy.ai/api/search-image?query=mobile%20app%20interface%20design%20for%20fitness%20tracking%2C%20clean%20UI%20design%20with%20health%20metrics%2C%20workout%20plans%2C%20activity%20tracking%20screens%2C%20modern%20mobile%20application%20design%2C%20user-friendly%20interface%2C%20fitness%20data%20visualization%2C%20progress%20tracking%20features%2C%20professional%20app%20design&width=600&height=400&seq=3&orientation=landscape"
                alt="Fitness App UI"
                class="w-full h-full object-cover object-top"
              />
              <div
                class="portfolio-overlay absolute inset-0 bg-primary/80 flex items-center justify-center p-6"
              >
                <div class="text-center text-white">
                  <h3 class="text-xl font-semibold mb-2">
                    FitTrack Mobile App
                  </h3>
                  <p class="mb-4">
                    A comprehensive fitness tracking application with
                    personalized workout plans and progress analytics.
                  </p>
                  <a
                    href="#"
                    class="inline-flex items-center text-white border-b border-white pb-1 hover:pb-2 transition-all"
                  >
                    View Details <i class="ri-arrow-right-line ml-1"></i>
                  </a>
                </div>
              </div>
            </div>
            <div class="p-6">
              <h3 class="text-lg font-semibold text-gray-900 mb-1">
                FitTrack Mobile App
              </h3>
              <p class="text-gray-600 text-sm mb-3">UI/UX Design</p>
              <a
                href="#"
                class="text-primary font-medium inline-flex items-center"
              >
                View Project <i class="ri-arrow-right-line ml-1"></i>
              </a>
            </div>
          </div>
                    <!-- Portfolio Item 3 -->
          <div
            class="portfolio-item bg-white rounded-lg overflow-hidden shadow-sm"
          >
            <div class="relative h-64">
              <img
                src="https://readdy.ai/api/search-image?query=computerSolutionswidth=600&height=400&seq=4&orientation=landscape"
                alt="Computer Solutions"
                class="w-full h-full object-cover object-top"
              />
              <div
                class="portfolio-overlay absolute inset-0 bg-primary/80 flex items-center justify-center p-6"
              >
                <div class="text-center text-white">
                  <h3 class="text-xl font-semibold mb-2">computers</h3>
                  <p class="mb-4">
                    An elegant website for a comprehesive computer solutions and IT consultation featuring
                    online reservations and digital menu.
                  </p>
                  <a
                    href="#"
                    class="inline-flex items-center text-white border-b border-white pb-1 hover:pb-2 transition-all"
                  >
                    View Details <i class="ri-arrow-right-line ml-1"></i>
                  </a>
                </div>
              </div>
            </div>
            <div class="p-6">
              <h3 class="text-lg font-semibold text-gray-900 mb-1">
                Saveur Restaurant
              </h3>
              <p class="text-gray-600 text-sm mb-3">Computer Solutions and IT Consultations</p>
              <a
                href="#"
                class="text-primary font-medium inline-flex items-center"
              >
                View Project <i class="ri-arrow-right-line ml-1"></i>
              </a>
            </div>
          </div>
          <!-- Portfolio Item 4 -->
          <div
            class="portfolio-item bg-white rounded-lg overflow-hidden shadow-sm"
          >
            <div class="relative h-64">
              <img
                src="https://readdy.ai/api/search-image?query=travel%20booking%20website%20interface%20with%20destination%20search%2C%20flight%20and%20hotel%20booking%20options%2C%20travel%20itinerary%20planner%2C%20vacation%20packages%20display%2C%20modern%20travel%20website%20design%2C%20user-friendly%20booking%20system%2C%20travel%20photography%20showcase%2C%20clean%20white%20background%20with%20accent%20colors&width=600&height=400&seq=5&orientation=landscape"
                alt="Travel Booking Platform"
                class="w-full h-full object-cover object-top"
              />
              <div
                class="portfolio-overlay absolute inset-0 bg-primary/80 flex items-center justify-center p-6"
              >
                <div class="text-center text-white">
                  <h3 class="text-xl font-semibold mb-2">Wanderlust Travel</h3>
                  <p class="mb-4">
                    A comprehensive travel booking platform with itinerary
                    planning and local experiences.
                  </p>
                  <a
                    href="#"
                    class="inline-flex items-center text-white border-b border-white pb-1 hover:pb-2 transition-all"
                  >
                    View Details <i class="ri-arrow-right-line ml-1"></i>
                  </a>
                </div>
              </div>
            </div>
            <div class="p-6">
              <h3 class="text-lg font-semibold text-gray-900 mb-1">
                Wanderlust Travel
              </h3>
              <p class="text-gray-600 text-sm mb-3">UI/UX, Development</p>
              <a
                href="#"
                class="text-primary font-medium inline-flex items-center"
              >
                View Project <i class="ri-arrow-right-line ml-1"></i>
              </a>
            </div>
          </div>
          <!-- Portfolio Item 5 -->
          <div
            class="portfolio-item bg-white rounded-lg overflow-hidden shadow-sm"
          >
            <div class="relative h-64">
              <img
                src="https://readdy.ai/api/search-image?query=real%20estate%20website%20design%20with%20property%20listings%2C%20interactive%20map%2C%20search%20filters%2C%20modern%20real%20estate%20platform%20interface%2C%20property%20details%20page%2C%20agent%20profiles%2C%20neighborhood%20information%2C%20professional%20real%20estate%20web%20design%20with%20clean%20white%20background&width=600&height=400&seq=6&orientation=landscape"
                alt="Real Estate Platform"
                class="w-full h-full object-cover object-top"
              />
              <div
                class="portfolio-overlay absolute inset-0 bg-primary/80 flex items-center justify-center p-6"
              >
                <div class="text-center text-white">
                  <h3 class="text-xl font-semibold mb-2">
                    PrimeEstate Properties
                  </h3>
                  <p class="mb-4">
                    A premium real estate platform with virtual tours and
                    neighborhood analytics.
                  </p>
                  <a
                    href="#"
                    class="inline-flex items-center text-white border-b border-white pb-1 hover:pb-2 transition-all"
                  >
                    View Details <i class="ri-arrow-right-line ml-1"></i>
                  </a>
                </div>
              </div>
            </div>
            <div class="p-6">
              <h3 class="text-lg font-semibold text-gray-900 mb-1">
                PrimeEstate Properties
              </h3>
              <p class="text-gray-600 text-sm mb-3">Web Design, Development</p>
              <a
                href="#"
                class="text-primary font-
