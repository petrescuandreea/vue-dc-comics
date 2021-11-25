<template>
    <div class="comic">
        <img :src="info.thumb" :alt="info.series">
        <h4 >{{info.series}}</h4>
    </div>
</template>

<script>
export default {
  name: 'Comiccard',
  props: {
    //   assegno a info il valore Object così so che tipo di dato mi verrà restituito
      info: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   .comic {
       width: calc(100% / 6 - 10px);
       margin: 20px 5px;
       cursor: pointer;

       img {
           width: 100%;
           height: 189px;
           object-fit: none;
           object-position: top;
           display: block;
       }

       h4 {
           width: 95%;
           font-size: 12px;
           font-weight: normal;
           text-transform: uppercase;
           margin: 10px 0;
       }
   }

</style>