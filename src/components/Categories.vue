<template>
    <div class="container">
                <div class="catebar">
                   <ul class="flex justify-se cateNav" >
                       <li><a href="/" class="active">All</a></li>
                       <li><a href="/">Action</a></li>
                       <li><a href="/">Drama</a></li>
                       <li><a href="/">Sci-fi</a></li>
                   </ul>
                </div>
                <div >
                    
                    <div class="row ai-c w-100">
                        <Cate v-for="movie in categories" v-bind:movie="movie" v-bind:key="movie.id" v-bind:class="movieClass"/>
                    </div>
                   <div  class="text-center mb-4">
                       <button class="p-1 r-curve btn-trans"><i class="fa fa-angle-down pr-1"></i>  Load More</button>
                   </div>
                </div>
            </div>
</template>

<script>
import Cate from "@/components/bits/Cate.vue"
export default {
    name:"Categories",
    props:["categories"],
    components:{
        Cate
    },
    data(){
         return {
            movieClass: "cat-outer p-relative mb-4 col-sm-12 col-md-6 col-lg-4"
         }
     },
}
</script>

<style scoped>
.cateNav{
        list-style:none;
        width:500px;
    }
</style>