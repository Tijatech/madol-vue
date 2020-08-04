<template>
    <div class="pb-6 pt-6">
        <div class="heading row ai-c pb-4">
            <h2 class="col-sm-12 col-md-3 col-lg-3">Featured</h2>
            <p class="col-sm-12 col-md-3 col-lg-5">This pick won't disappoint you</p>
        </div>
        <div class="row justify-sb ai-c">
            <div v-on:click="scrollLeft"><i class="fa fa-angle-left fa-2x"></i> </div>
            <div class="flex justify-sb ai-c col-10 overflow-auto hide-scroll" width="100%" id="box">
                <Movie v-for="movie in featured" v-bind:movie="movie" v-bind:key="movie.id" v-bind:imgWidth="imgWidth" v-bind:movieClass="movieClass"/>
            </div>
            <div v-on:click="scrollRight"><i class="fa fa-angle-right fa-2x p-1"></i> </div>
        </div>
    </div>
</template>


<script>
var  left = 0;
import Movie from "@/components/bits/Movie.vue"
export default {
     name:"Featured",
     props: ["featured"],
     components:{
         Movie
     },
     data(){
         return {
            movieClass: "mov-outer p-relative mr-5",
            imgWidth: "350px"
         }
     },
     methods: {
        
         scrollLeft: () => {      
                var box = document.querySelector("#box");
                if(left > 0){left-=100}
                box.scroll({
                left: left,
                behavior: 'smooth'
            })
        },
        scrollRight: () => {      
            var box = document.querySelector("#box")
            if(left < box.scrollWidth){left+=100}
            box.scroll({
            left: left,
            behavior: 'smooth'
        })
        }
     }
    
    
}
</script>