<template lang="jade">
.wrap
 .tips.login(v-if="$store.state.layer.loging_status")
  icon.fa-spin(name="spinner",style="color:#e4a941;width:3rem;height:1.8rem;")
 .tips(v-else) {{$store.state.layer.main_message}}
</template>
<style lang="scss">
  .main_layer{
  	 width:100%;
  	 height:100%;
  	 position:absolute;
  	 top:0;
  	 z-index:100;
     .wrap{
      display:-webkit-flex;
      justify-content: center;
     }
     .login{
       top:8rem;
       background-color:rgba(0,0,0,.14) !important;
       width:3rem;
       padding:0.5rem 0.5rem 0.1rem 0.5rem !important;
       margin:0 !important;
     }
  	 .tips,.tips_2{
  	 	background-color:rgba(247,183,70,0.8);
  	 	color:#fff;
      text-shadow:0rem 0.08rem 0.3rem rgba(0,0,0,0.5);
  	 	position:relative;
  	 	z-index:200;
  	 	padding:0 1rem;
  	 	margin:0 auto;
  	 	line-height:1.5rem;
      top:11rem;
      border-radius: 0.18rem;
      letter-spacing: 0.05rem;
  	 }
  }
</style>
