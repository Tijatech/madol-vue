<template>
  <div class="home">
    <Slider v-bind:slider="home.slider"/>
    <main>
        <Featured v-bind:featured="home.featured"/>
        <NewArrival v-bind:newarrival="home.newarrival"/>
        <ComingSoon />
    </main>
  </div>
</template>

<script>
// @ is an alias to /src
import Slider from '@/components/Slider.vue';
import Featured from '@/components/Featured.vue';
import NewArrival from '@/components/NewArrival.vue';
import ComingSoon from '@/components/ComingSoon.vue';

export default {
  name: 'Home',
  components: {
    Slider,
    Featured,
    NewArrival,
    ComingSoon
  },
  data(){
    return {

      home:{
      slider:{
        urls:[
          "https://image-cdn.essentiallysports.com/wp-content/uploads/20200626165844/Untitled-design-1-2-1600x900.jpg"
        ],
        title: [
          "Avengers",
          "END GAME"
        ],
      },
      featured:[
          {
            id:1,
            img: 'https://www.screengeek.net/wp-content/uploads/2019/08/terminator-dark-fate.jpg',
            title: "Terminator"
          },
          {
            id:2,
            img: 'https://upload.wikimedia.org/wikipedia/en/f/fe/1917_%282019%29_Film_Poster.jpeg',
            title: "Time"
          },
          {
            id:3,
            img: 'https://www.screengeek.net/wp-content/uploads/2018/12/venom-movie.jpg',
            title: "Venom"
          },
          {
            id:4,
            img: 'https://upload.wikimedia.org/wikipedia/en/f/fe/1917_%282019%29_Film_Poster.jpeg',
            title: "Time"
          },
          {
            id:5,
            img: 'https://www.screengeek.net/wp-content/uploads/2018/12/venom-movie.jpg',
            title: "Venom"
          }   
      ],
      newarrival:[
        {
          id:1,
          img: 'https://image.tmdb.org/t/p/w500/sJKcpT5LRuCdGpWm29yH2bMWqT0.jpg',
          title: "Hacker"
        },
        {
          id:2,
          img: 'https://upload.wikimedia.org/wikipedia/en/f/fe/1917_%282019%29_Film_Poster.jpeg',
          title: "Time"
        },
        {
          id:3,
          img: 'https://www.screengeek.net/wp-content/uploads/2018/12/venom-movie.jpg',
          title: "Venom"
        },
        {
          id:4,
          img: 'https://image.tmdb.org/t/p/w500/sJKcpT5LRuCdGpWm29yH2bMWqT0.jpg',
          title: "Hacker"
        },
        {
          id:5,
          img: 'https://upload.wikimedia.org/wikipedia/en/f/fe/1917_%282019%29_Film_Poster.jpeg',
          title: "Time"
        },
        {
          id:6,
          img: 'https://www.screengeek.net/wp-content/uploads/2018/12/venom-movie.jpg',
          title: "Venom"
        }  
    ],
            
    }
    }
  }
    
  
}
</script>
