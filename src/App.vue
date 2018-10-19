<template>
  <div>
    <app-header></app-header>
    <app-nerds></app-nerds>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Nerds from './components/Nerds.vue';

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-nerds': Nerds
  },
  data () {
    return {
      
    }
  }
}
</script>

<style>

</style>
