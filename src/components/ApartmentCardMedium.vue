<template>
    <a href="#SomeLink">
          <!-- Showcase IMG -->
          <div class="relative pr-30/100 bg-gray-300">
            <img class="select-none absolute w-full h-full object-cover" :src="apartments.img_link" alt="">
          </div>
          <!-- Showcase IMG -->

          <!-- Right Side of IMG Container-->
          <div class="bg-gray-300 px-3">

            <!-- Title -->
            <div class="flex items-center justify-between text-2xl pt-2">
              <h1 class="font-bold text-indigo-900">{{apartments.title}}</h1>
              <p class="font-semibold text-teal-500">${{apartments.cost}}
                <span class="text-indigo-300">/
                  {{apartments.per}}</span>
              </p>
            </div>

            <p class="text-lg font-semibold text-indigo-600 leading-4">{{apartments.baths}}
              Baths &bull;
              {{apartments.rooms}}
              Rooms &bull;
              {{apartments.size}}
              m²</p>
            <!-- Title -->

            <!-- Description -->
            <div class="mt-5 mb-5">
              <p class="text-sm text-gray-600 font-semibold">{{apartments.description}}</p>
            </div>
            <!-- Description -->

            <!-- Rating and Contact -->
            <div class="mb-4 flex justify-between">
              <!-- Rating Cirles -->
              <div class="flex flex-wrap mt-2 items-center justify-between">
                <div class="flex items-center">
                  <div v-for="i in 5" :key="i"
                    :class="i <= apartments.rating ? 'bg-teal-400' : 'border-2 border-teal-400'"
                    class="rounded-full w-4 h-4 mr-2"></div>
                  <p class="ml-2 mr-2 font-semibold text-xs text-indigo-300 select-none">
                    <a href="#Reviews">{{apartments.reviews}} reviews</a>
                  </p>
                </div>
              </div>
              <!-- Rating Cirles -->

              <!-- Contact SVG's -->
              <div class="flex items-center justify-center">
                <a href="#Phone" class="mr-1">
                  <svg class="w-7 h-7" xmlns="http://www.w3.org/2000/svg" width="19.5" height="19.5"
                    viewBox="0 0 19.5 19.5">
                    <path
                      d="M3,4.944A1.944,1.944,0,0,1,4.944,3H8.133a.972.972,0,0,1,.922.665l1.456,4.368a.972.972,0,0,1-.488,1.176l-2.194,1.1a10.735,10.735,0,0,0,5.363,5.363l1.1-2.194a.972.972,0,0,1,1.176-.488l4.368,1.456a.972.972,0,0,1,.665.923v3.188A1.944,1.944,0,0,1,18.556,20.5h-.972A14.584,14.584,0,0,1,3,5.917Z"
                      transform="translate(-2 -2)" fill="none" stroke="#4fd1c5" stroke-linecap="round"
                      stroke-linejoin="round" stroke-width="2" /></svg>
                </a>
                <a href="#Mail" class="ml-3 mr-2 ">
                  <svg class="w-7 h-7" xmlns="http://www.w3.org/2000/svg" width="20.773" height="16"
                    viewBox="0 0 20.773 16">
                    <path
                      d="M3,8l7.89,5.26a2,2,0,0,0,2.22,0L21,8M5,19H19a2,2,0,0,0,2-2V7a2,2,0,0,0-2-2H5A2,2,0,0,0,3,7V17A2,2,0,0,0,5,19Z"
                      transform="translate(-1.613 -4)" fill="none" stroke="#4fd1c5" stroke-linecap="round"
                      stroke-linejoin="round" stroke-width="2" /></svg>
                </a>
              </div>
              <!-- Contact SVG's -->
            </div>
            <!-- Rating and Contact -->
          </div>
          <!-- Right Side of IMG Container -->
    </a>
</template>

<script>
    export default {
        props: ['apartments']
    }
</script>