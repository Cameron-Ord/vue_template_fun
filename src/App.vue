<template>
  <div id="the_true_parent">
    <header id="page_header"><page-header></page-header></header>
    <main id="page_main"><page-main></page-main>
    </main>
    <footer id="page_footer"><page-footer></page-footer></footer>
  </div>
</template>

<script>

import PageHeader from './components/PageHeader.vue';
import PageFooter from './components/PageFooter.vue';
import PageMain from './components/PageMain.vue';
export default {
  name: 'App',
  components: {

PageFooter,
PageHeader,
PageMain
  }
}
</script>

<style>
*{
  padding: 0px;
  margin: 0px;
}

body{


}

#page_header{

  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

  min-height: 10vh;

  justify-items: center;

  align-items: center;
}

#page_main{

  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  
  min-height: 80vh;

  justify-items: center;

  align-items: center;
}

#page_footer{

  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

  min-height: 80vh;

  justify-items: center;

  align-items: center;
}
</style>
