<template>
  <div>
    <about-top />
    <about-bottom />
  </div>
</template>

<script>
import AboutTop from '@/components/AboutTop'
import AboutBottom from '@/components/AboutBottom'

export default {
  name: 'About',
  components: {
    'about-top': AboutTop,
    'about-bottom': AboutBottom
  }
}
</script>
