<template>
    <div class="mb-6 mt-6">
        <div class="heading row ai-c pb-4">
            <h2 class="col-sm-12 col-md-3 col-lg-3">New Arrival</h2>
            <p class="col-sm-12 col-md-3 col-lg-5">This pick won't disappoint you</p>
        </div>
        <div>
                    
            <div class="row ai-c">
                <Movie v-for="movie in newarrival" v-bind:movie="movie" v-bind:key="movie.id" imgWidth="100%" v-bind:class="movieClass"/>  
            </div>
            <div  class="text-center">
                <button class="p-1 r-curve btn-trans"><i className="fa fa-angle-down pr-1"></i>  Load More</button>
            </div>
        </div>
    </div>
</template>


<script>
import Movie from "@/components/bits/Movie.vue"
export default {
    name:"NewArrival",
    props: ["newarrival"],
     components:{
         Movie
     },
     data(){
         return {
            movieClass: "mov-outer-alt p-relative mb-4 col-xs-12 col-sm-12 col-md-6 col-lg-4",
            imgWidth: "100%",
         }
     }
}
</script>


<style scoped>

</style>