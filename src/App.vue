<template>
<div>
  <div>
    <router-link to="/about">about</router-link>
    <router-link to="/products">products</router-link>
  </div>
  <router-view></router-view>
</div>
</template>

<script>
import VueRouter from "vue-router"
import about from "./about.vue"
import products from "./products.vue"

export default{
  router:new VueRouter({
    routes:[
      {
        path:"/about",
        component: about
      },{
        path:"/products",
        component: products
      }
    ]
  })
}
</script>
<style>

</style>