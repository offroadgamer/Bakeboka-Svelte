<script>
    
</script>

<div class="navbar">
    <div class="navbar-title">
<<<<<<< HEAD:src/routes/about/Navbar.svelte
        <h2><a class="navbar-icon" href="/">Bakeboka</a></h2>
=======
        <h2><a class="navbar-icon" href="./src/App.svelte">Bakeboka</a></h2>
>>>>>>> main:src/lib/Navbar.svelte
    </div>
    <div class="navbar-searchbar">
        <div class="searchbar-box">
            <p class="searchbar-text">Søk...</p>
            <img class="search-icon" src="./src/lib/images/search_icon.png" alt="bigger jigger">
        </div>
    </div>
    <div class="navbar-burgermeny">
        <div class="burger-line"></div>
        <div class="burger-line"></div>
        <div class="burger-line"></div>
    </div>
</div>

<style>
    a {
        text-decoration: none;
        color: #111111; 
    }

    a:hover {
        color: #888888;
    }

    .navbar {
        background-color: #FFE59F;
        width: 100%;
        min-height: 100px;
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
        margin: 0px 20px;
    }

    .searchbar-box {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        padding: 0px 20px;
    }
    .search-icon {
        max-height: 40px;
        margin: auto 0px auto auto;
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