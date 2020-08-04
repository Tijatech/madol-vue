<template>
    <div v-bind:class="movieClass">
        <img v-bind:src="movie.img" v-bind:alt="movie.title" width="100%"  height="200"/>
        <div class="mov-inner movStyle" >
            <div class="mov-details">
                <h2>{{movie.title}}</h2>
                <div><small>Action X X X X X</small></div>
            </div>                    
        </div>
    </div>
</template>

<script>
export default {
    name:"Cate",
    props: ["movie","movieClass"]
}
</script>

<style scoped>
    .movStyle{
        position:absolute;
        width:100%;
        top:0;
        height:100%;
        padding:0 20px  20px 20px;
        background:rgba(0, 0, 0, 0.452);
        display:flex;
        align-items:flex-end;
    }
    
</style>