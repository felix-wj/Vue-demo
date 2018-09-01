<template>
    <div>
      这是购物车页面
      <span>商品id:{{$route.query.goodsId}}</span>
      <span>商品id:{{$route.params.goodsId}}</span>
    </div>

</template>

<script>
    export default {
        name: "Cart"
    }
</script>

<style scoped>

</style>
