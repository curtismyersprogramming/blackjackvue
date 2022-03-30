<template>
    <main class="game-area">
        <section class="dealer-area">
        </section>
        <section class ="player-area">
        </section>
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
  min-height: 12.4rem;
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
</style>