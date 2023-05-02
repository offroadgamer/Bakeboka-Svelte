<script>
    import Footer from "./lib/Footer.svelte";
    import Navbar from "./lib/Navbar.svelte";
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
            <img class="oppskrift-img" src="../../img/dagens_oppskrift.jpg" alt="mat">
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
                <li>Varm melken til 37 grader og ha i en bakebolle sammen med egg og gjær. 
                    Bland sammen til gjæren er løst opp. Dersom du bruker tørrgjær skal 
                    denne blandes med de tørre ingrediensene.</li>
                <li>Ha i sukker, hvetemel, kardemomme og salt. Elt i 10 minutter.</li>
                <li>Ha i smøret i terninger og elt til deigen slipper bollen og du kan 
                    «strekke» deigen uten av den ryker. Dette tar ytterligere ca 10-15 
                    minutter.</li>
                <li>La deigen heve i ca 45 minutter.</li>
                <li>Bland sammen smør, brunt sukker og kanel.</li>
                <li>Strø litt mel utover bakebordet og ta deigen ut av bakebollen. Kjevle 
                    deigen til et rektangel, ca 20x25 cm. Smør på fyllet, og rull deigen 
                    sammen som en lang pølse.</li>
                <li>Fordel 1/3 av karamellsausen utover en dyp langpanne med høye kanter. 
                    Dekk gjerne formen med bakepapir før du har i karamellsausen.</li>
                <li>Skjær deigpølsen i skiver og legg skivene i en langpanne med høye 
                    kanter dekket med bakepapir.</li>
                <li>Dekk til bollene med plastfolie og la heve i 30 minutter. Ha over 
                    halvparten av karamellsausen som er igjen.</li>
                <li>Stek bollene på 225 grader, midt i ovnen, i ca 10 minutter til de er 
                    gylne.</li>
                <li>Ha resten av karamellsausen og de hakkede pistasjnøttene over de 
                    nybakte bollene med en gang de tas ut av ovnen.</li>
            </ol>
        </div>
    </div>
    <Footer></Footer>
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

    .oppskrift-img-box {
        min-width: 55vw;
    }

    .oppskrift-img {
        width: 100%;
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
        min-height: 200px;
        padding: 20px;
        line-height: 2;
        margin-bottom: 100px;
    }

    .oppskrift-specs-header {
        font-size: 35px;
    }

    .oppskrift-specs-list-item {
        font-size: 20px;
    }
</style>