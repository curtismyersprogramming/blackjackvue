<template>
    <main class="game-area">
        <section class="dealer-area">
            <img src="./png/2_of_clubs.png" alt="2 of clubs">
            <img src="./png/6_of_clubs.png" alt="6 of clubs">
        </section>
        <section class ="player-area">
            
            <img src="./png/2_of_clubs.png" alt="2 of clubs">
            <img src="./png/6_of_clubs.png" alt="6 of clubs">
            
            
            
        </section>
        <div class='playercontrol'>
            <player-control-area/>
        </div>
        <div class="info-area">
              
                <div class="info-bar">
                    <div class="grid-item">Dealers Hand: {{ dealerValue }} </div>
                    <div class="grid-item-feedback">Select an option to recieve feedback</div>
                    <div class="grid-item">
                       
                        <p class="bank-up">+</p>
                        <p class="bet-value">100</p>
                        <p class="bank-down">-</p>
                    </div>
                    <div class="grid-item">
                        Running Count: +2<br>
                        Cards remaining: 212<br>
                        True Count: +1
                                        
                    </div>
                    <div class="grid-item">Dealers Hand: {{ playerValue }}</div>

                    </div>
                </div>
    </main>
</template>

<script>
import PlayerControlArea from './PlayerControlArea.vue'





export default {
    name: 'gamePlayArea',
    components:{
        PlayerControlArea,
       
       
    },
    data(){
        
        return{
            dealerValue: 8,
            playerValue: 8
        }
    }
    
    
        
    
}
</script>

<style scoped>
    .game-area{
        min-height: 88vh;
        display: flex;
        flex: 1;
        flex-direction: column;
        z-index: 50;
        background-color: red;
    }

    .dealer-area {
  
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-items: center;
  min-height: 15.4rem;
  background-color: blueviolet;
}
.player-area {
  flex: 1 0;
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-items: center;
  background-color: blue;
}

.info-area{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 120px;
}

.info-bar{
    display: grid;
    justify-items: center;
    align-items: center;
    background-color: #111111;
    width: 95%;
    height: 85%;
    border-radius: 15px;
    grid-template-columns: 20% 20% 20% 20% 20%;
    color: white;
    font-weight: bold;
    

    
    
    
    
}

.grid-item{
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    width: 100%;
    height: 100%;
    
    
}

.grid-item-feedback{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    background: green;
}

img{
    width:7rem;
    margin-right: 10px;
   
}

</style>