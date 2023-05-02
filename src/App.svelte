<script>
    import { each } from "svelte/internal";
    import Navbar from "./lib/Navbar.svelte";
    import Footer from "./lib/Footer.svelte";
    import Cake from "./oppskrift_kategorier/Cake.svelte";
    import YeastBakery from "./oppskrift_kategorier/Yeast_bakery.svelte";
    import Bread from "./oppskrift_kategorier/Bread.svelte";
    

    const cakeList = [
        {name: "Bløtkake", 
        link: "./bløtkake.svelte"},

        {name: "Eplepai", 
        link: "./Eplepai.svelte"},

        {name: "Oreokake", 
        link: "./oreokake.svelte"},

        {name: "Sjokoladekake",
        link: "./sjokoladekake.svelte"}
    ]

    const yeast_bakeryList = [
        {name: "Kanelbolle"},
        {name: "Hvetebolle"},
        {name: "Sticky Buns"},
        {name: "Skolebrød"}
    ]

    const breadList = [
        {name: "Fiberbrød"},
        {name: "Kornbrød"},
        {name: "Muslibrød"},
        {name: "Norsk bygg"}
    ]
</script>


<body>
    <Navbar></Navbar>
    <div class="main">
        <div class="dagens-oppskrift">
            <a href="./src/Oppskrift.svelte">
                <h1>Dagens oppskrift:</h1>
                <img src="./img/dagens_oppskrift.jpg" alt="mat">
                <h2>Sticky buns med karamellsaus</h2>
            </a>
    </div>
        <div class="andre-oppskrifter">
            <div class="oppskrift-liste">
                <h3>Kaker:</h3>
                <ul>
                    {#each cakeList as cake}
                    <Cake cake={cake}></Cake>
                    {/each}
                </ul>
            </div>
            <div class="oppskrift-liste">
                <h3>Gjærbakst:</h3>
                <ul>
                {#each yeast_bakeryList as yeast_bakery}
                    <YeastBakery yeast_bakery={yeast_bakery}></YeastBakery>
                {/each}
                </ul>
            </div>
            <div class="oppskrift-liste">
                <h3>Brødvarer:</h3>
                <ul>
                {#each breadList as bread}
                    <Bread bread={bread}></Bread>
                {/each}
                </ul>
            </div>
        </div>   
    </div>
    <Footer></Footer>
</body>


<style>

    .main {
        width: 80vw; 
        margin: auto;
        margin-top: 100px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .dagens-oppskrift {
        max-width: 70%;
        display: flex;
        justify-content: center;
        padding: 10px 40px;
        margin: auto auto 50px;
        box-shadow:  10px 10px 26px #cccccc,
                -10px -10px 26px #ffffff;
    }

    .andre-oppskrifter {
        width: 70%;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        
    }

    .oppskrift-liste {
        padding: 10px 20px;
        width: 23%;
        height: 300px;
        box-shadow:  10px 10px 26px #cccccc,
                -10px -10px 26px #ffffff;
    }
</style>