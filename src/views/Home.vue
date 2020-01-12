<template>
  <div class="home">
    <Header />
    <Home />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from '@/components/Home.vue'

import Header from '@/components/Header.vue'

export default {
  name: 'home',
  components: {
    Home,
    Header
  }
}
</script>
