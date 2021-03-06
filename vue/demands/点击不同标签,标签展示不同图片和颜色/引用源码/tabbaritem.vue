<template>

  <div class="tabbaritem" @click="itemclick()">
  <div>
      
	  <slot v-if="isactive" name="itemimg"></slot>
	  <slot v-else  name="itemimgactive"></slot>
    <div  :style="activestyle"><slot  name="itemdiv"></slot></div>
	  
  </div>


  </div>

</template>

<script>
export default {
  name: 'tabbarItem',
  data(){
           return{
                   }
             },
    computed:{
         isactive() { return this.$route.path.indexOf(this.link) !== -1},
         activestyle(){return this.isactive ? {color:this.activecolor} : {}}
          },         
    props: {
                  link: {type: String,required: true},
                  activecolor:{type: String,default:'red'}
              },

 
    methods:{
      itemclick(){
      this.$router.replace(this.link)

      }
    
    }         
}
</script>

<style scoped>




.tabbaritem{
flex:1;
margin-bottom: 30px;
}

.tabbaritem img{
width:24px;
height:24px;
margin-top:10px;
    vertical-align: middle;
}

.tabbaritem div a{
display:block;
margin-top:0px;
}


</style>
