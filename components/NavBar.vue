<template xmlns="http://www.w3.org/1999/html">
  <div class="sticky top-0 left-0 border-8 border-amber-400">
    <nuxt-link to="/">
      <img src="/header_image.jpg"/>
    </nuxt-link>
    <ul class="flex justify-around border-t-8 border-t-amber-400 py-2">
      <li>
        <nuxt-link to="/" :class="$nuxt.$route.path === '/' && 'text-purple-300'">
          <i>Home</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/artists" :class="$nuxt.$route.path === '/artists' && 'text-purple-300'">
          <i>Artists</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/events" :class="$nuxt.$route.path === '/events' && 'text-purple-300'">
          <i>Events</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/studio" :class="$nuxt.$route.path === '/studio' && 'text-purple-300'">
          <i>Studio</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/contact" :class="$nuxt.$route.path === '/contact' && 'text-purple-300'">
          <i>Contact</i>
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    selected: { type: String, default: '' }
  }
}
</script>

<style scoped>

</style>
