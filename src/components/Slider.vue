<template>
    <div>
                <div class="outer-layer">
                    <img v-bind:src="slider.urls[0]"
                    alt="" width="100%" height="100%"/>
                     <div class="inner-layer row">
                        <div class="details col-sm-12 col-lg-6">
                            <div>
                                <h1>{{slider.title[0]}}</h1>
                                <h3>{{slider.title[1]}}</h3>
                            </div>
                            <div>
                                <div>Action | <s>X X X X X</s> | 2020</div>
                                <p>
                                    The Rock seizes the opportunity of a lifetime when 
                                    she lands a job with the world's most powerful 
                                    technology and social media company.
                                </p>
                            </div>
                            <div>
                                <a href="/watch" class="watch-link"><i class="fa fa-play-circle"></i> Watch Now</a>
                            </div>
                        </div>

                     </div>
                </div>
            </div>
</template>

<script>

export default {
    name:"Slider",
    props:["slider"],

}

</script>

<style scoped>

</style>