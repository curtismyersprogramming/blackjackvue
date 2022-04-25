<template>
    <header>
       <nav>
            <ul class="nav_links">
                <li><a href="#">Rules</a></li>
                <li class="maintitle">Blackjack</li>
                <li><a href="#">Card Counting</a></li>
                
            </ul>
            
        </nav>
    </header>
</template>

<script>


export default {
    name: 'Navbar-item',
    components:{
       

    }
};

</script>

<style scoped>

li,a{
    text-decoration: none;
    list-style: none;
    color: white;
}
header{
    display: flex;
    justify-content: center;
    background-color: rgb(0, 0, 0);
    height: 5vh;
    width: 100%;
    align-items: center;
    padding: 30px 10%;
    color: white;

}

.nav_links li{
    display: inline-block;
    padding: 0px 20px;
}

.nav_links li a{
    transition: all 0.3s ease 0s;
}
.nav_links li a:hover{
    color: gold;
}

.maintitle{
    font-weight: bold;
    font-size: 26px;
}

</style>