<template>
  <div id="app">
    <v-head></v-head>
    <v-article></v-article>
    <v-footer></v-footer>
  </div>
</template>

<script>
  (function(i,s,o,g,r,a,m){i["DaoVoiceObject"]=r;i[r]=i[r]||function(){(i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;a.charset="utf-8";m.parentNode.insertBefore(a,m)})(window,document,"script",('https:' == document.location.protocol ? 'https:' : 'http:') + "//widget.daovoice.io/widget/15a4e0ff.js","daovoice");
  import article from './components/Article';
  import head from './components/Header';
  import footer from './components/Foote';
export default {
  name: 'App',
  data(){
    return{
      msg:"你好Vue",
    }
  },
  components:{
    "v-head":head,
    'v-article':article,
    'v-footer':footer,
  }
}
</script>

<style>
  @import "https://cdn.staticfile.org/twitter-bootstrap/3.3.0/css/bootstrap.min.css";
  @import  "../static/css/index.css";
  @import  "../static/css/code.css";
</style>
