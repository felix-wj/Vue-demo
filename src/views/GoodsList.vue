<template>
  <div>商品列表
    <span>{{$route.params.goodsId}}</span><br>
    <router-link to="/goods/title">显示商品标题</router-link>
    <router-link to="/goods/image">显示商品图片</router-link>
    <div>
      <router-view></router-view>
    </div>
    <router-link v-bind:to="{name:'cart',params:{goodsId:123}}">去购物车</router-link>
    <button v-on:click="jump">去购物车</button>
  </div>

</template>

<script>
    export default {
      data(){
          return{
            msg:'hello'
          }
      },
      methods:{
        jump(){
          // this.$router.push("/cart")
          this.$router.push({path:'/cart?goodsId=1'})
        }
      }
    }
</script>

