<template>
  <div id="app">
    <Header />
    <Snow 
      :active='true'
      :zIndex='2'
      :wind='1' 
      :swing='3' 
      :speed='l' 
      color="#FFFFFF"/>
  </div>
</template>

<script>
import Header from './components/Vue_Header.vue';
import Snow from '../node_modules/vue-niege/src/Snow.vue';

export default {
  name: 'app',
  data() {
    return{
      
    }
  },
  components:{
    Header,
    Snow,
  }
}
</script>

<style lang="scss">
/*Обнуление*/
* {padding: 0;margin: 0;border: 0;}
*,*:before,*:after {-moz-box-sizing: border-box;-webkit-box-sizing: border-box;box-sizing: border-box;}
:focus,:active {outline: none;}
a:focus,a:active {outline: none;}
nav, footer, header, aside {display: block;}
html, body{height: 100%;width: 100%;font-size: 100%;line-height: 1;font-size: 14px;-ms-text-size-adjust: 100%;-moz-text-size-adjust: 100%;-webkit-text-size-adjust: 100%;}
input,button,textarea {font-family: inherit;}
input::-ms-clear{display: none;}
button{cursor: pointer;}
button::-moz-focus-inner{padding: 0;border: 0;}
a, a:visited{text-decoration: none;}
a:hover{text-decoration: none;}
ul li{list-style: none;}
img {vertical-align: top;}
h1,h2,h3,h4,h5,h6{font-size: inherit;font-weight: 400;}
/*----------------------------*/

.warning{
  text-align: center;
  font-size: 20px;
  margin:20px 0 0 0;
  color: #DC143C;
}

.choice{
  display: flex;
  margin:50px auto 0 auto;
  max-width: 1300px;

  &-choice{
    width: 100%;
    color: $color2;
    font-size: 18px;
    text-align: center;
  }

  &-art{
    width: 500px;
    margin: 0px 50px 0px 30px;
    border: 3px solid $color3;
    border-radius: 20%;
  }
}

body{
  background-color: $color1;
}

</style>