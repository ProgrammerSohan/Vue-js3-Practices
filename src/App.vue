<template lang="html">

  <p>Welcome to vue3</p>
  <HelloWorldComponent :title="title" />
  <CardComponent title="Header 1" description="1111 Lorem cupidatat eiusmod Lorem cupidatat eiusmod Lorem cupidatat eiusmod." />
 <!--
   <CardComponent title="Header 2" description="2222 Lorem cupidatat eiusmod Lorem cupidatat eiusmod Lorem cupidatat eiusmod. "/>
  <CardComponent title="Header 3" description="3333 Lorem cupidatat eiusmod Lorem cupidatat eiusmod Lorem cupidatat eiusmod. "/>
  <CardComponent title="Header 4" description="4444 Lorem cupidatat eiusmod Lorem cupidatat eiusmod Lorem cupidatat eiusmod. "/>
    <CardComponent title="New Header 1" description="5555 Lorem cupidatat eiusmod Lorem cupidatat eiusmod Lorem cupidatat eiusmod. "/>
 -->
    
    <LayoutComponent>

     
      <CardComponent title="Header 1" description="1111 Lorem cupidatat eiusmod Lorem cupidatat eiusmod Lorem cupidatat eiusmod. "/>
      
     
      <template v-slot:afterFooter>
        <p>&copy; Maestro</p>

      </template >

    </LayoutComponent>

</template>

<script lang="js">
import HelloWorldComponent from './components/HelloWorldComponent.vue';
import CardComponent from './components/CardComponent.vue';
import LayoutComponent from './components/LayoutComponent.vue';


export default {
  name: 'App',
  components: {
    HelloWorldComponent,
    CardComponent,
    LayoutComponent

  },
  data(){
    return{
      title: "Vuejs Learning 4"
    }
  }
}
</script>

<style lang="css">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
