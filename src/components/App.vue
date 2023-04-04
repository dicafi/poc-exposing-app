
<template>
  <div>
    <router-view />

    <ExposedComponent />

	<br />
	 A demo of a single page application made in Vue.js, PostCSS and Bootstrap

  </div>
</template>

<script>
  import ExposedComponent from './ExposedComponent.vue'

  export default {
    components: {
      ExposedComponent,
    }
  }
</script>
