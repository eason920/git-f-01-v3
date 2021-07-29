<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <Card :title-cpn="title2"/>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
  components: {
    Card
  },
  created () {
    console.log('api is ', process.env.VUE_APP_API)
  },
  data () {
    return {
      title2: process.env.VUE_APP_PATH
    }
  }
}
</script>
