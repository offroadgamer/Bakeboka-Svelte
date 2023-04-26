<script>
    
</script>

<div class="navbar">
    <div class="navbar-title">
        <h2><a class="navbar-icon" href="./Oppskrift.svelte">Bakeboka</a></h2>
    </div>
    <div class="navbar-searchbar">
        <div class="searchbar-box">
            <p class="searchbar-text">Søk...</p>
        </div>
    </div>
    <div class="navbar-burgermeny">
        <div class="burger-line"></div>
        <div class="burger-line"></div>
        <div class="burger-line"></div>
    </div>
</div>

<style>
    .navbar {
        background-color: #FFE59F;
        width: 100%;
        height: 100px;
        top: 0px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        box-shadow:  10px 10px 32px #f2f2f2,
                -10px -10px 32px #ffffff;
    }

    .navbar-title {
        font-size: 20px;
        padding-left: 20px;
    }

    .navbar-icon {
        font-weight: 600;
    }

    .navbar-searchbar {
        background-color: #FFFFFF;
        height: 50px;
        width: 400px;
        border-radius: 30px;
        padding-left: 20px;
    }
    
    .navbar-burgermeny {
        display: flex;
        flex-direction: column;
        padding-right: 20px;
    }

    .burger-line {
        background-color: #111111;
        height: 5px;
        width: 50px;
        margin: 5px;
    }
</style>