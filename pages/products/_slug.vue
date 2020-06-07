<template>
  <div>
    <product-top />
    <!-- <product-mid /> -->
    <product-bottom />
  </div>
</template>

<script>
import ProductTop from '@/components/ProductTop'
import ProductMid from '@/components/ProductMid'
import ProductBottom from '@/components/ProductBottom'

export default {
  name: 'Product',
  components: {
    'product-top': ProductTop,
    'product-mid': ProductMid,
    'product-bottom': ProductBottom
  }
}
</script>
