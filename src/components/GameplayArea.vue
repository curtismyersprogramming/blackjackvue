<template>
    <main class="game-area">
        <section class="dealer-area">
            <h1>Dealer</h1>
        </section>
        <section class ="player-area">
            
            <h1>Player</h1>
            
            
        </section>
        <div class='playercontrol'>
            <player-control-area/>
        </div>
        <div class="info-area">
              
                <div class="info-bar">
                    <div class="grid-item">Dealers Hand: 19</div>
                    <div class="grid-item-feedback">Feedback</div>
                    <div class="grid-item">Bank</div>
                    <div class="grid-item">Count Values</div>
                    <div class="grid-item">Players Hand</div>

                    </div>
                </div>
    </main>
</template>

<script>
import PlayerControlArea from './PlayerControlArea.vue'

export default {
    name: 'gamePlayArea',
    components:{
        PlayerControlArea
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
  justify-content: space-around;
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
    
    
    
}

.grid-item{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    font-weight: bold;
    
}

.grid-item-feedback{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    background: green;
}

</style>