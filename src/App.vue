<template>
  <div id="app">

    <body class="font-Montserrat">

      <!-- ApartmentCard SM - MD -->
      <div class="md:hidden">
        <div class="flex justify-center" v-for="apartments in Apartments" :key="apartments">
          <div class="shadow-md max-w-xl bg-gray-300 mx-2 pb-2 my-3 rounded-xl overflow-hidden">
            <a href="#SomeLink">
              <Apartment-card :apartments="apartments" />
            </a>
          </div>
        </div>
      </div>
      <!-- ApartmentCard SM - MD-->

      <!-- ApartmentCard MD - LG-->
      <div class="hidden md:contents lg:hidden">
        <!-- Root -->
        <div class="flex my-8 mx-3 rounded-2xl overflow-hidden shadow-md" v-for="apartments in Apartments"
          :key="apartments">

          <!-- Showcase IMG -->
          <div class="relative pr-30/100 bg-gray-300">
            <img class="select-none absolute w-full h-full object-cover" :src="apartments.img_link" alt=""></div>
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
                    <a href="#Reviews">{{apartments.reviews}}
                      reviews</a>
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
        </div>
        <!-- Root -->
      </div>
      <!-- ApartmentCard MD - LG-->

    </body>
  </div>
</template>

<script>
  import ApartmentCard from './components/ApartmentCard'
  export default {
    name: 'App',
    components: {
      ApartmentCard
    },
    data() {
      return {
        Apartments: [{
          title: 'Manhattan Tower in NYC',
          img_link: 'https://images.unsplash.com/photo-1470219556762-1771e7f9427d?ixlib=rb-1.2.1&ixid' +
            '=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1489&q=80',
          baths: 4,
          rooms: 8,
          size: 560,
          cost: 1250,
          per: 'Week',
          rating: 4,
          reviews: 256,
          description: 'The Presidio Residences offer a unique opportunity to live in a national park se' +
            'tting and enjoy quiet neighborhoods, convenient location, beautiful open spaces,' +
            ' and outstanding recreational amenities. Call today to see your new home at The ' +
            'Presidio Residences.'
        }, {
          title: 'Jerrys Appartments NYC',
          img_link: 'https://images.unsplash.com/photo-1527267207156-3372670819dc?ixlib=rb-1.2.1&ixid' +
            '=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
          baths: 1,
          rooms: 5,
          size: 368,
          cost: 150,
          per: 'Day',
          rating: 3,
          reviews: 434,
          description: "Tower 28 located in Long Island City, NY rises above the rest with 58 floors of " +
            "sophisticated floor plans and impressive amenities. Tower 28 brings new elegance" +
            " to the area’s already historic, industrial charm. A short two minute walk from " +
            "Tower 28 puts residents at the doorstep of Queensboro Plaza. The plaza provides " +
            "easy access to rail and bus lines. There's the N, W and 7 trains that transfer r" +
            "esidents to points all across Queens to Manhattan"
        }, {
          title: 'Summer House - Stamford',
          img_link: 'https://images.unsplash.com/photo-1490644658840-3f2e3f8c5625?ixlib=rb-1.2.1&ixid' +
            '=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1534&q=80',
          baths: 4,
          rooms: 10,
          size: 432,
          cost: 1535,
          per: 'Week',
          rating: 4,
          reviews: 126,
          description: 'WE OFFER IN-PERSON & VIRTUAL TOURS, VIDEOS & 3D INTERACTIVE FLOOR PLANS Living a' +
            't the DVORA Art House provides the right balance of comfort and convenience, rig' +
            'ht in the heart of Downtown Jersey City. A unique boutique building with great a' +
            'menities such as city view rooftop with a pool & BBQ, Fitness center with Peloto' +
            'n bikes and more. '
        }, {
          title: 'Art House Apartments',
          img_link: 'https://images.unsplash.com/photo-1542855596-45eb2695c74c?ixlib=rb-1.2.1&ixid=ey' +
            'JhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=676&q=80',
          baths: 2,
          rooms: 9,
          size: 439,
          cost: 200,
          per: 'Week',
          rating: 5,
          reviews: 141,
          description: "DVORA is more than managers of your space, we're caretakers of the community. Wh" +
            "en choosing to live in the DVORA Art House, you can rest assured that you will b" +
            "e taken care of. From quality construction & gorgeous design to speedy customer " +
            "service, virtual events & considerate in-unit services, we're confident you will" +
            " LOVE being at home."
        }]
      }
    }
  }
</script>