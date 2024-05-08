<template>
  <main>
    <header class="relative">
      <div>
        <nav class="relative z-50">
          <div class="nav-container">
            <div class=" nav-content">
              <div class="absolute toggle-btn-div">
                <button type="button" @click="toggleMenu"
                  class="relative">
                  <svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                    aria-hidden="true">
                    <path stroke-linecap="round" stroke-linejoin="round"
                      d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                  </svg>
                  <svg class="hidden h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                    aria-hidden="true">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                  </svg>
                </button>
              </div>
              <div class="navlinks-container">
                <div class="flex flex-shrink-0 items-center">
                  <img class="h-8 w-auto" src="./assets/img/Logo.png" alt="Your Company">
                </div>
                <div class="hidden sm:ml-6 relative sm:block">
                  <div class="flex items-center space-x-4">
                    <a href="#"
                      class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">ABOUT US</a>
                    <a href="#"
                      class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">CONTACT US</a>
                    <a href="#"
                      class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium"><img src="./assets/img/topicon (1).png" alt=""></a>
                    <a href="#"
                      class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium"><img src="./assets/img/topicon (2).png" alt=""></a>
                  </div>
                </div>
              </div>

            </div>
          </div>

          <!-- Mobile menu, show/hide based on menu state. -->
          <div class="absolute w-full backdrop-blur-sm" id="mobile-menu" :class="{ 'hidden': !isMenuOpen }">
            <div class="space-y-1 px-2 pb-3 pt-2">
              <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
              <a href="#" class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium"
                aria-current="page">Dashboard</a>
              <a href="#"
                class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Team</a>
              <a href="#"
                class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Projects</a>
              <a href="#"
                class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Calendar</a>
            </div>
          </div>
        </nav>
      </div>
      <img class="topleftmask" src="./assets/img/topmask.png" alt="" />
      <img class="topgradient absolute z-10 top-0 right-0" src="./assets/img/topgradient.png" alt="" />
      <img class="banner-img top-0" src="./assets/img/banner-img1.png" alt="" />

      <div class="flex relative items-center h-full">
        <div class=" px-12 mt-14">
          <div class="flex flex-col">
            <span class="text-4xl md:text-7xl header-text text-white uppercase">Lorem ipsum</span>
            <span
              class="uppercase header-text bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent text-4xl md:text-7xl">amet
              consetur</span>
          </div>
          <p class="text-white mt-4 text-xl max-w-xl pb-10">
            Lorem ipsum dolor sit amet consectetur. Nisl proin cras sapien sed
            lorem amet scelerisque.
          </p>
          <!-- <button class="btn px-16 py-5 w-fit mt-4">Button</button> -->
          <button class="w-fit mx-auto my-3">
            <img src="./assets/img/button.svg" alt="" />
          </button>
          <ul class="space-x-2 mb-10 flex mt-5">
            <li class="pr-6 bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent">
              <span class="text-xl font-bold">120k+</span>
              <p class="text-white text-sm">Lorem ipsum dolor ipsum</p>
            </li>
            <li
              class="border-gradient border-l-2 px-6 border-l-white  bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent">
              <span class="text-xl font-bold">10k+</span>
              <p class="text-white text-sm">Lorem ipsum dolor</p>
            </li>
            <li
              class="border-gradient border-l-2 px-6 border-l-white  bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent">
              <span class="text-xl font-bold">22%</span>
              <p class="text-white text-sm">Lorem ipsum</p>
            </li>
          </ul>
        </div>
      </div>
    </header>
    <section class="min-h-screen flex justify-center items-center">
      <div class="grid md:grid-cols-2 grid-cols-1">
        <div class="relative h-fit w-fit">
          <img src="./assets/img/network.png" alt="" />
          <img class="absolute top-[22%] right-[18%] h-[12%]" src="./assets/img/img-object1.png" alt="" />
          <img class="absolute top-[16%] left-[25%] h-[8%]" src="./assets/img/img-object2.png" alt="" />
          <img class="absolute bottom-[34%] left-[17%] h-[10%]" src="./assets/img/img-object3.png" alt="" />
          <img class="absolute bottom-[22%] right-[19%] h-[10%]" src="./assets/img/img-object4.png" alt="" />
          <img class="absolute bottom-[8%] right-[45%] h-[9%]" src="./assets/img/img-object5.png" alt="" />
        </div>
        <div class="flex justify-center items-center">
          <img src="./assets/img/light.png" class="absolute right-0" alt="" />
          <div class="relative z-2 flex flex-col md:px-12 px-2">
            <span class="md:text-6xl text-3xl uppercase header-text text-white">Lor Ipsum is</span>
            <div>
              <span
                class="header-text uppercase bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent md:text-6xl text-3xl">simply
              </span>
              <span class="header-text md:text-7xl uppercase text-3xl text-white">dummyr</span>
            </div>
            <p class="text-white mt-4 md:text-xl text-md max-w-xl">
              Lorem ipsum dolor sit amet consectetur. Nisl proin cras sapien sed
              lorem amet scelerisque.Lorem ipsum dolor sit amet consectetur.
              Nisl proin cras sapien sed lorem amet scelerisque.
            </p>
            <!-- <button class="btn px-16 py-5 w-fit mt-4">Button</button> -->
            <button class="w-fit mx-auto mt-4">
              <img src="./assets/img/button.svg" alt="" />
            </button>
          </div>
        </div>
      </div>
    </section>
    <section class=" relative">
      <div class=" space-y-10">
        <img src="./assets/img/Union.png" class="absolute right-0 top-32" alt="">
        <div class="relative z-2 flex  flex-col md:px-20 px-2">
          <span class="md:text-7xl  text-3xl uppercase header-text text-white">Phasellus nec ligula</span>
          <div>
            <span class="header-text md:text-6xl uppercase text-3xl text-white">non felis </span>
            <span
              class="header-text uppercase bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent md:text-6xl text-3xl">imperdiet
            </span>

          </div>
          <span class="md:text-6xl uppercase text-3xl header-text text-white">commodo .</span>
        </div>
        <div class="grid md:grid-cols-3 grid-cols-1 mx-auto md:px-20 px-2 gap-5 relative">
          <div class="bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] p-[2px] rounded-xl">
            <div
              class="bg-gradient-to-b px-14 text-white h-full from-[#1A0645] to-[#1A0645] flex flex-col justify-between rounded-xl p-5 space-y-5">
              <div>
                <img class="mx-auto py-10" src="./assets/img/card-object1.png" alt="">
              </div>
              <div class="space-y-2">
                <h2 class="font-bold text-xl">Travel Safety</h2>
                <p class="text-white text-lg">Lorem ipsum Nisl dolor sit amet conse Nisl ctetur. Nisl proin cras sapien
                  sed Lorem.</p>
              </div>
              <button class="mx-auto">
                <img src="./assets/img/button.svg" alt="" />
              </button>

            </div>
          </div>
          <div class="bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] p-[2px] rounded-xl">
            <div
              class="bg-gradient-to-b px-14 text-white h-full from-[#1A0645] to-[#1A0645] rounded-xl p-5 flex flex-col justify-between space-y-5">
              <div>
                <img class="mx-auto py-10" src="./assets/img/card-object2.png" alt="">
              </div>
              <div class="space-y-2">
                <h2 class="font-bold text-xl">eScooter & Bikes</h2>
                <p class="text-white text-lg">Lorem ipsum Nisl dolor sit amet conse Nisl ctetur. Nisl proin cras sapien
                  sed Lorem.</p>
              </div>
              <button class="mx-auto">
                <img src="./assets/img/button.svg" alt="" />
              </button>

            </div>
          </div>
          <div class="bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] p-[2px] rounded-xl">
            <div
              class="bg-gradient-to-b px-14 text-white h-full from-[#1A0645] to-[#1A0645] rounded-xl flex flex-col justify-between p-5 space-y-5">
              <div class="">
                <img class="mx-auto py-10" src="./assets/img/card-object3.png" alt="">
              </div>
              <div class="space-y-2">
                <h2 class="font-bold text-xl">Evacuation</h2>
                <p class="text-white text-lg">Lorem ipsum Nisl dolor sit amet conse Nisl ctetur. Nisl proin cras sapien
                  sed Lorem.</p>
              </div>
              <button class="mx-auto">
                <img src="./assets/img/button.svg" alt="" />
              </button>

            </div>
          </div>

        </div>
      </div>
    </section>
    <section
      class="relative bg-[url(./assets/img/footer-image.png)] bg-cover bg-center h-screen flex items-center justify-center">
      <div class="relative z-100 w-full justify-center items-center ">
        <!-- <img class=" h-full absolute w-full" src="./assets/img/footer-image.png" alt=""> -->
        <div class="relative flex justify-center flex-col">
          <div class="uppercase header-text text-center">
            <span class="text-6xl header-text text-white">Register</span><br />
            <span class="text-6xl header-text text-white">your </span>
            <span
              class="header-text bg-gradient-to-r from-[#C327BC] via-[#333CF0] to-[#00FAFE] bg-clip-text text-transparent text-6xl">school
            </span>
            <span class="text-6xl header-text text-white">Today</span>

          </div>
          <p class="text-white text-center my-5">Create safety ambassadors for today & tomorrow.</p>
          <button class="mx-auto">
            <img src="./assets/img/button.svg" alt="" />
          </button>
        </div>
      </div>
    </section>
    <section class="relative flex items-center py-5 justify-center">
      <div class="flex gap-10 flex-wrap md:flex-nowrap md:px-20 px-3 w-full">
        <div class="space-y-5 text-white flex flex-col justify-between">
          <img src="./assets/img/Logo.png" alt="">
          <div>
            <p>© Copyright 2024</p>
            <p class="text-xs">Hashinclude, All rights reserved.</p>
          </div>
        </div>
        <div class="flex w-full flex-col">
          <div class="flex justify-between flex-wrap whitespace-nowrap">
            <div class="grid grid-cols-3 md:grid-cols-3 gap-10 text-sm text-white">
              <ul class="space-y-4 mb-10">
                <li class="border-gradient border-gradient border-l-2 px-5 border-l-white">Option 1</li>
                <li class="border-gradient border-l-2 px-5 border-l-white">Option 2</li>
              </ul>
              <ul class="space-y-4 mb-5">
                <li class="border-gradient border-l-2 px-5 border-l-white">Option 1</li>
                <li class="border-gradient border-l-2 px-5 border-l-white">Option 2</li>
              </ul>
              <ul class="space-y-4 mb-5">
                <li class="border-gradient border-l-2 px-5 border-l-white">Option 1</li>
                <li class="border-gradient border-l-2 px-5 border-l-white">Option 2</li>
              </ul>
            </div>
            <div class="py-5">
              <img src="./assets/img/logoright.png" alt="">
            </div>
          </div>
          <hr class="hr-gradient">
          <div class="flex justify-between items-center mt-3">
            <div class="space-x-10 text-xs mt-3 sociel-links">
              <span
                class="hover:bg-gradient-to-r text-white  hover:from-[#C327BC] hover:via-[#333CF0] hover:to-[#00FAFE] hover:bg-clip-text hover:text-transparent">facebook</span>
              <span
                class="hover:bg-gradient-to-r text-white  hover:from-[#C327BC] hover:via-[#333CF0] hover:to-[#00FAFE] hover:bg-clip-text hover:text-transparent">Twitter</span>
              <span
                class="hover:bg-gradient-to-r text-white  hover:from-[#C327BC] hover:via-[#333CF0] hover:to-[#00FAFE] hover:bg-clip-text hover:text-transparent">Instagram</span>
              <span
                class="hover:bg-gradient-to-r text-white  hover:from-[#C327BC] hover:via-[#333CF0] hover:to-[#00FAFE] hover:bg-clip-text hover:text-transparent">Youtube</span>
            </div>
            <div class="hidden md:block">
              <img src="./assets/img/dashboard.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
<script>
export default {
  data() {
    return {
      isMenuOpen: false
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
};
</script>
<style>


</style>
