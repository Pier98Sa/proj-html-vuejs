<template>
    <header>
        <div class="navbar-top">
            
        </div>
        <div class="navbar-bottom">
            
        </div>         
    </header>
  
</template>

<script>
export default {
    name:'MyHeader',

}
</script>

<style lang="scss" scoped>

    header{
        position: fixed;
        width: 100%;
        top: 0;
        left: 0;
        
    }
    .navbar-top{
        height: 30px;
        background-color: grey;
    }
    .navbar-bottom{
        height: 90px;
        background-color: black;
    }

</style>