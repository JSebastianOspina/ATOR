<template>
  <div class="l">
    
    <div class="flex items-center justify-center bg-fixed w-screen bg-center bg-cover" :style="'background-image: url(orquidea1.jpg);height:'+altura+'px'">
        
        <h3 class="text-5xl text-gray-300 font-bold">
        ATO
    </h3>
    </div>
    
    
  </div>
</template>

<script>
export default {
    mounted (){
        this.altura = screen.height;

    },
    data(){
        return{
            altura:'800'
        }
    }
}
</script>

<style>

</style>