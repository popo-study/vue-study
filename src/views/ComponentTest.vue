<template>
  <div>
    <img alt="Vue logo" src="../../public/assets/logo.png">
    <v-button 
    @btn-click="btnClick" 
    :class="btnClass"
    :buttonName="name">
    </v-button>
  </div>
</template>

<script>

export default {
  name: 'component_test',
  data() {
    return {
      name: 'button',
      btnClass: ''
    };
  },  
  methods: {
    btnClick(className) {
      if(this.btnClass==''){
        this.btnClass = className;
      }else{
        this.btnClass = '';
      }
    }
  },
  components: {}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
