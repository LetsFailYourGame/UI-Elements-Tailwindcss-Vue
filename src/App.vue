<template>
  <div id="app" class="h-full bg-gray-100">
    <body class="font-Montserrat">

      <div class="md:hidden">
        <div class="flex justify-center" v-for="apartments in Apartments" :key="apartments">
          <div class="shadow-md max-w-xl bg-gray-300 mx-2 pb-2 my-3 rounded-xl overflow-hidden"> 
            <a href="#SomeLink">
              <Apartment-card :apartments="apartments" />
            </a>      
          </div>
        </div>
      </div>

    </body>
  </div>
</template>

<script>
import ApartmentCard from './components/ApartmentCard'
export default {
  name: 'App',
  components: {
    ApartmentCard,
  },
  data() {
    return {
      Apartments: [
        {
          title: 'Manhattan Tower in NYC',
          img_link: 'https://images.unsplash.com/photo-1470219556762-1771e7f9427d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1489&q=80',
          baths: 4,
          rooms: 8,
          size: 560,
          cost: 1250,
          per: 'Week',
          rating: 4,
          reviews: 256,
          description: 'The Presidio Residences offer a unique opportunity to live in a national park setting and enjoy quiet neighborhoods, convenient location, beautiful open spaces, and outstanding recreational amenities. Call today to see your new home at The Presidio Residences.',
        },
        {
          title: 'Jerrys Appartments NYC',
          img_link: 'https://images.unsplash.com/photo-1527267207156-3372670819dc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80',
          baths: 1,
          rooms: 5,
          size: 368,
          cost: 150,
          per: 'Day',
          rating: 3,
          reviews: 434,
          description: "Tower 28 located in Long Island City, NY rises above the rest with 58 floors of sophisticated floor plans and impressive amenities. Tower 28 brings new elegance to the area’s already historic, industrial charm. A short two minute walk from Tower 28 puts residents at the doorstep of Queensboro Plaza. The plaza provides easy access to rail and bus lines. There's the N, W and 7 trains that transfer residents to points all across Queens to Manhattan",
        },
        {
          title: 'Summer House - Stamford',
          img_link: 'https://images.unsplash.com/photo-1490644658840-3f2e3f8c5625?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1534&q=80',
          baths: 4,
          rooms: 10,
          size: 432,
          cost: 1535,
          per: 'Week',
          rating: 4,
          reviews: 126,
          description: 'WE OFFER IN-PERSON & VIRTUAL TOURS, VIDEOS & 3D INTERACTIVE FLOOR PLANS Living at the DVORA Art House provides the right balance of comfort and convenience, right in the heart of Downtown Jersey City. A unique boutique building with great amenities such as city view rooftop with a pool & BBQ, Fitness center with Peloton bikes and more. ',
        },
        {
          title: 'Art House Apartments',
          img_link: 'https://images.unsplash.com/photo-1542855596-45eb2695c74c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=676&q=80',
          baths: 2,
          rooms: 9,
          size: 439,
          cost: 200,
          per: 'Week',
          rating: 5,
          reviews: 141,
          description: "DVORA is more than managers of your space, we're caretakers of the community. When choosing to live in the DVORA Art House, you can rest assured that you will be taken care of. From quality construction & gorgeous design to speedy customer service, virtual events & considerate in-unit services, we're confident you will LOVE being at home.",
        },
    ]
    }
  }
}
</script>

