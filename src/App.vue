<template>
  <div id="app">
    <body class="font-Montserrat">

      <!-- Wrapper -->
      <div>
        <div v-for="apartments in Apartments" :key="apartments">
          
          <!-- ApartmentCard-Small -->
          <div class="md:hidden flex justify-center">
            <Apartment-card :apartments="apartments" class="shadow-md max-w-xl bg-gray-300 mx-2 pb-2 my-3 rounded-xl overflow-hidden"/>
          </div>
          <!-- ApartmentCard-Small -->
          
          <!-- ApartmentCard-Medium -->
          <div class="hidden md:contents lg:hidden">
            <ApartmentCardMedium :apartments="apartments" class="flex my-8 mx-3 rounded-2xl overflow-hidden shadow-md"/>      
          </div>
          <!-- ApartmentCard-Medium -->

        </div>
      </div>
      <!-- Wrapper -->

    </body>
  </div>
</template>

<script>
  import ApartmentCard from './components/ApartmentCard'
  import ApartmentCardMedium from './components/ApartmentCardMedium'

  export default {
    name: 'App',
    components: {
      ApartmentCard,
      ApartmentCardMedium
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