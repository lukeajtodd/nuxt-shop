<template>
  <div>
    <hero />
    <products :products="allProduct" />
  </div>
</template>

<script>
import Hero from '@/components/Hero.vue'
import Products from '@/components/Products.vue'
import getProducts from '@/queries/getProducts'

export default {
  apollo: {
    allProduct: {
      prefetch: true,
      query: getProducts
    }
  },
  components: {
    hero: Hero,
    products: Products
  }
}
</script>
