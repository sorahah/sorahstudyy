<template>
  <testTxt :username="username" :numberOfVisit="numberOfVisit" />
  <ul>
    <listfor :item="item"/>
  </ul>
</template>
<script >
import testTxt from './components/testtxt.vue';
import listfor from './components/listfor.vue';
export default {
    name:"App",
    components:{
      testTxt,
      listfor
    },
    data(){
      return{
        username: "뿡뿡",
        numberOfVisit: 20,
        item:['치킨','피자','불닭']
      }
    }
}
</script>
<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
