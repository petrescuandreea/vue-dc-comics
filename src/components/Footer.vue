<template>
    <div>
        <FooterUp/>
        <FooterCenter/>
        <FooterBottom/>
    </div>
    
</template>

<script>
import FooterUp from '../components/FooterUp.vue';
import FooterCenter from '../components/FooterCenter.vue';
import FooterBottom from '../components/FooterBottom.vue';


export default {
  name: 'Footer',
  components: {
      FooterUp,
      FooterCenter,
      FooterBottom
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>