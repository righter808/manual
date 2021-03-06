<template>
 <div>

  <router-view></router-view>

     
   <tabbar>
                <tabbaritem link="/home" activecolor="red">
<div slot="itemdiv">首页</div>
    
	   <img slot="itemimg" src="@/assets/img/tabbar/20210121112257.jpg" alt=""></img>
	   <img slot="itemimgactive" src="@/assets/img/tabbar/handsome/QQ截图20210122101403.jpg" alt=""></img>
               
	
	 </tabbaritem>
	 <tabbaritem  link="/find" activecolor="red">
	   <div slot="itemdiv">发现</div>
	   <img slot="itemimg" src="@/assets/img/tabbar/QQ截图20210121113518.jpg" alt=""></img>
 <img slot="itemimgactive" src="@/assets/img/tabbar/handsome/QQ截图20210122101502.jpg" alt=""></img>
	 </tabbaritem>
	 <tabbaritem  link="/cate" activecolor="blue">
	   <div slot="itemdiv">购物车</div>
	   <img slot="itemimg" src="@/assets/img/tabbar/QQ截图20210121113528.jpg" alt=""></img>
<img slot="itemimgactive" src="@/assets/img/tabbar/handsome/QQ截图20210122101510.jpg" alt=""></img>
	 </tabbaritem>
	 <tabbaritem  link="/my" activecolor="blue">
	   <div slot="itemdiv">我的</div>
	   <img slot="itemimg" src="@/assets/img/tabbar/QQ截图20210121113538.jpg" alt=""></img>
<img slot="itemimgactive" src="@/assets/img/tabbar/handsome/QQ截图20210122101517.jpg" alt=""></img>
	 </tabbaritem>
	


  </tabbar>
   
 </div>
</template>

<script>
import tabbar from '@/components/common/tabbar'
import tabbaritem from '@/components/common/tabbaritem'
import textbar from '@/components/common/textbar'

export default {
  name: 'tabbarmain',
  components: {tabbar,tabbaritem},
  data(){
           return{
  
                 
              
                   
                     }
             },
}
</script>

<style>
@import "../assets/css/base.css"

</style>
