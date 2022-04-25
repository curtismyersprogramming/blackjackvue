<template>
<div class="button-area">
    <Button  @click="isVisible=true"  v-if="!isVisible" class="deal-button"     text="Deal" color="grey"/>
    <div v-if="isVisible" class = GameplayButtons>
    <Button class="double-button"   text="Double Down"/>
    <Button class="hit-button"      text="Hit"/>
    <Button class="stand-button"    text="Stand"/>
    <Button class="split-button"    text="Split"/>
    </div>
</div>
    
</template>         

<script>

import Button from './Button.vue'


export default {
    name:'playerControlArea',
    components:{
    Button,
    },
    data: function() {
        return {
            isVisible: false
        }
    },
    methods:{
       
        
    },
}
</script>

<style scoped>
.button-area{
    display: flex;
    align-content: center;
    justify-content: center;
    height: 60px;
    background: black;
}

.deal-button{
    width: 250px;
}

.GameplayButtons{
    display: flex;
    align-content: center;
    justify-content: center;
    background: black;
}

button{
    font-weight: bold;
}
.hit-button{
    width: 250px;
    background: green;
}
.stand-button{
    width: 250px;
    background: red;
}
.double-button{
    width: 250px;  
    background: blue;
}
.split-button{
    width: 250px;
    background: goldenrod;
}



</style>