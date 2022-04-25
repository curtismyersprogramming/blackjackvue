<template>
<Navbar />
 <div class="container">
    <Gameplay-area />
  </div>
</template>

<script>
import Navbar from './components/Navbar'
import GameplayArea from './components/GameplayArea.vue'



export default {
  name: 'App',
  components: {
    Navbar,
    GameplayArea,
   
    
  },
  data() {
    return{
    isGameRunning:false,
    }
  },
  methods: {
    startGame(){
      this.isGameRunning =true;
      console.log("game is true");

    }
  }

 
}
</script>


<!-- Global Styles -->
<style>

/*Poppins font*/
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Poppins', sans-serif;
  background-color: #111111;
  
}
.container {
  max-width: 95%;
  margin: 10px auto;
  overflow: auto;
  min-height: 90vh;
  padding: 10px;
  border-radius: 5px;
  background-color: #ffffff;
}
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
.btn:focus {
  outline: none;
}
.btn:active {
  transform: scale(0.98);
}
.btn-block {
  display: block;
  width: 100%;
}
</style>
