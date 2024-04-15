<template>
  <div id="app"> 
   <HeaderComponent message="waaa"/>
   <div class="main-content">

      <HelloWorld msg="salim " />
      <MainComponent message="azdiiiin salim">
        <router-view> </router-view>
      </MainComponent>
    </div>
  <FooterComponent message="je suis le footer"/>
      
   </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import FooterComponent from './components/layout/FooterComponent.vue'
import MainComponent from './components/layout/MainComponent.vue'
import HeaderComponent from './components/layout/HeaderComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    HelloWorld,
    FooterComponent,
    MainComponent,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
