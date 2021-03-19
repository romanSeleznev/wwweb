<template>
  <v-carousel v-model="model"
    hide-delimiter-background="true"
    height="100%"
    vertical="true"
    :continuous="false"
    vertical-delimiters
     v-scroll.self="onScroll" 
  >
      <v-carousel-item
      
      >
        <PartMain/>
      </v-carousel-item>
      <v-carousel-item
      >
        <PartAbout/>
      </v-carousel-item>
      <v-carousel-item
      >
        <PartForm/>
      </v-carousel-item>
  </v-carousel>
</template>

<script>
import PartMain from './Parts/PartMain'
import PartAbout from './Parts/PartAbout'
import PartForm from './Parts/PartForm'
export default {
    name: 'Page',
    components:{
        PartMain,
        PartAbout,
        PartForm
    },
    data: function(){
        return{
            model: 0
        }
    },
    methods:{
        onScroll () {
        this.model++
      }
    }
}
</script>

<style>

</style>