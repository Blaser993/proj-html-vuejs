<template>
  <div>
    <Header></Header>
  </div>
    
</template>

<script>
import Header from "./components/Header.vue";

	export default {
    
    components:{
      Header,
    }


	}
</script>

<style lang="scss"> //senza scoped in App.vue
  @use "./style/general.scss"
</style>
