<template>
  <section class="text-gray-700 body-font">
    <div class="container px-5 py-24 mx-auto">
      <div class="flex flex-wrap -m-4">
        <div
          v-for="product in products"
          :key="product._id"
          class="lg:w-1/4 md:w-1/2 p-4 w-full"
        >
          <a class="block relative h-48 rounded overflow-hidden">
            <img
              alt="ecommerce"
              class="object-cover object-center w-full h-full block"
              src="https://dummyimage.com/420x260"
            />
          </a>
          <div class="mt-4">
            <h3 class="text-gray-500 text-xs tracking-widest title-font mb-1">
              CATEGORY
            </h3>
            <h2 class="text-gray-900 title-font text-lg font-medium">
              {{ product.title }}
            </h2>
            <p class="mt-1">${{ price(product) }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Products',
  props: {
    products: {
      type: Array,
      required: true
    }
  },
  computed: {
    price() {
      return product => product.defaultProductVariant.price
    }
  }
}
</script>
