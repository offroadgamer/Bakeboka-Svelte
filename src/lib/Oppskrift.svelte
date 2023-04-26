<script>
    import Navbar from "./Navbar.svelte";
</script>

<head>
    <meta charset="UTF-8">
    <link rel="icon" type="image/svg+xml" href="/icon.png" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Bakeboka</title>
</head>

<body>
    <Navbar></Navbar>
    <div class="oppskrift">
        <div class="oppskrift-title">
            <h1>Sticky buns med karamellsaus</h1>
        </div>
        <div class="oppskrift-img-box">
            <img src="../../img/dagens_oppskrift.jpg" alt="mat">
        </div>
        <div class="oppskrift-specs">
            <div class="ingredienser">
                <h2 class="oppskrift-specs-header">Ingredienser:</h2>
                <ul>
                    <li class="oppskrift-specs-list-item">5 dl melk</li>
                    <li class="oppskrift-specs-list-item">1 stk egg</li>
                    <li class="oppskrift-specs-list-item">50 g fersk gjær</li>
                    <li class="oppskrift-specs-list-item">150 g sukker</li>
                    <li class="oppskrift-specs-list-item">1 kg hvetemel</li>
                    <li class="oppskrift-specs-list-item">1 ss kardemomme</li>
                    <li class="oppskrift-specs-list-item">1 ts salt</li>
                    <li class="oppskrift-specs-list-item">125 g smør i terninger, romtemperert</li>
                </ul>
            </div>
            <div class="utstyr">
                <h2 class="oppskrift-specs-headrr">Utstyr:</h2>
                <ul>
                    <li class="oppskrift-specs-list-item">Kjele</li>
                    <li class="oppskrift-specs-list-item">Bakebolle</li>
                    <li class="oppskrift-specs-list-item">Sleiv</li>
                    <li class="oppskrift-specs-list-item">Langpanne</li>
                    <li class="oppskrift-specs-list-item">Plastfolie</li>
                </ul>
            </div>
        </div>
        <div class="how-to-do">
            <h2>Slik gjør du:</h2>
            <ol>
                <li>Ha smør, sukker, kremfløte og honning i en kjele. Kok opp og la 
                    koke i ca 5 minutter til karamellsausen tykner. Dra kjelen av varmen 
                    og vend inn saltet.</li>
            </ol>
        </div>
    </div>
    
</body>

<style>
    .oppskrift {
        width: 70vw;
        margin: auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        font-family: Inter, system-ui, Avenir, Helvetica, Arial, sans-serif;
        line-height: 1.5;
        font-weight: 400;
    }

    .oppskrift-title {
        text-align: center;
        width: 100%;
        margin-bottom: 30px;
        font-size: 20px;
    }

    .oppskrift-specs {
        display: flex;
        flex-direction: row;
        width: 100%;
        padding: 10px;
        margin: auto;
    }

    .ingredienser {
        width: 50%;
        border: 5px solid pink;
        margin: 10px;
        min-height: 200px;
        padding: 20px;
    }

    .utstyr {
        width: 50%;
        border: 5px solid green;
        margin: 10px;
        min-height: 200px;
        padding: 20px;
    }

    .how-to-do {
        border: 5px solid blue;
        width: 100%;
        height: 200px;
        padding: 20px;
    }

    .oppskrift-specs-header {
        font-size: 35px;
    }

    .oppskrift-specs-list-item {
        font-size: 20px;
    }
</style>