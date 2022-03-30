<template>
    <button :style="{background: color}" class="btn">{{text}}</button>
</template>

<script>
export default{
    name:'Button-item',
    props:{
        text:String,
        color:String
    }
}
</script>
