<template>
    <div class="carousel">
        <slot></slot>
        <button class="carousel_nav carousel_next" @click.prevent="next">Suivant</button>
         <button class="carousel_nav carousel_Pprev" @click.prevent="prev">Precedent</button>
    </div>
</template>

<script>
    export default{
        
        data(){
           
            return{
                index:0,
                slides: [],
            }
        },
        mounted(){
           this.slides = this.$children
           this.slides.forEach((slide,i)=>{
               slide.index = i
           })
        },
        methods:{
            next(){
                this.index++;
            },
            prev(){
                this.index--;
            }
        }
    }
</script>
<style>

</style>