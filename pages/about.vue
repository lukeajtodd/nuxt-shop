<template>
  <div>
    <about-top />
    <about-mid />
    <about-bottom />
  </div>
</template>

<script>
import AboutTop from '@/components/AboutTop'
import AboutMid from '@/components/AboutMid'
import AboutBottom from '@/components/AboutBottom'

export default {
  name: 'About',
  components: {
    'about-top': AboutTop,
    'about-mid': AboutMid,
    'about-bottom': AboutBottom
  }
}
</script>
