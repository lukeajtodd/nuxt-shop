<template>
  <div>
    <main-header />
    <main>
      <nuxt />
    </main>
    <main-footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Layout',
  components: {
    'main-header': Header,
    'main-footer': Footer
  }
}
</script>
