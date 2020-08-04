<template>
  <div class="series">
   <Slider v-bind:slider="series.slider"/>
   <main>
        <Categories v-bind:categories="series.all"/>       
    </main>
  </div>
</template>



<script>
import Slider from '@/components/Slider.vue';
import Categories from '@/components/Categories.vue';

export default {
  name:"Series",
  components:{
    Slider,
    Categories
  },
  data(){
    return {
  
      
    series:{
      slider:{
        urls:[
          "https://images.justwatch.com/backdrop/10573937/s1440/the-dark-tower",
          "https://www.joblo.com/newsimages1/avengers-infinity-war-main.jpg"
        ],
        title: [
          "Dark Tower",
          ""
        ]
      },
      all:[
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
