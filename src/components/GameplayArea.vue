<template>
    <main class="game-area">
        <section class="dealer-area">
            <h1>Dealer</h1>
        </section>
        <section class ="player-area">
            
            <h1>Player</h1>
            
            
        </section>
        <div class="info-area">
              
                <div class="info-bar">
                    <div class="grid-item">Dealers Hand</div>
                    <div class="grid-item">Feedback</div>
                    <div class="grid-item">Bank</div>
                    <div class="grid-item">Count Values</div>
                    <div class="grid-item">Players Hand</div>

                    </div>
                </div>
    </main>
</template>

<script>
export default {
    
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
    grid-template-columns: auto auto auto auto auto;
    color: white;
    
    
}
</style>