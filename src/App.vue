<template>
  <div>
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
    
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";

	export default {
    
    components:{
      Header,
      Footer,
      Main
    }


	}
</script>

<style lang="scss"> //senza scoped in App.vue
  @use "./style/general.scss"
</style>
