<script>
    import { createEventDispatcher } from 'svelte';
    import Button from "../shared/Button.svelte";
    import Hoverable from './Hoverable.svelte';
 </script>

<section>
    <img src="/img/New Beat.jpg" alt="portada New Beat" class="nb"><br>
    <h3 class="blue">New Beat: bombos & estrobos</h3><br>
</section>       
    <p>Madrid, 1991, Km. 15,500 de una carretera cualquiera. Cuatro historias underground: 
        bombos, estrobos, mescalinas y unos pocos discos mágicos... Y los aviones sobrevolando 
        un inolvidable chalet blanco, en el que se esconde el mejor club de música electrónica 
        de toda la historia de la capital.<br><br>
        "La presión en el Infierno es total, con todo dios bailando como si fuera la última 
        mañana de la historia; así que doblo la apuesta para intentar saltar la banca… 
        Coloco el disco, y ya al hacer la preescucha se me pone la piel de gallina: 
        bombo roto, riff de guitarra rock, voces tribales indias… A tumba abierta. 
        Allá va el Our Reservation, de Desperation. La reacción de la peña es increíble: 
        un espectáculo total, electrizante (“¡ueeeeeeeeee, aaaaaaaah…!”). 
        El suelo de la cabina se mueve bajo mis pies, mientras algunos tíos se acercan para 
        chocarme la mano. El bombo y la guitarra siguen reventando la pista; es como si este tema 
        estuviera hecho a medida para esta gente. La batalla es total. La gente salta en todas 
        direcciones; la mezcla de sudor, alcohol y maría invade la cabina. 
        (“¡ueeeeeeeeee, aaaaaaaah…!”).<br><br>
        Ahora desaparecen todos los elementos del Our Reservation, excepto la guitarra, que 
        ametralla en todas direcciones. La gente se vuelve loca. ¿Qué meto ahora? ¿Bajo un 
        poco el ritmo, o lo aumento hasta que la peña termine tirando las jaulas al suelo? 
        Decido seguir mis impulsos: jugármelo todo al rojo infierno... Pongo el disco y ajusto 
        el pitch. Atrás, adelante. Atrás, adelante… Y lo lanzo: el trepidante 8-15, de RMZ. 
        Y más chillidos. Y la peña, saltando hasta el techo. Y las jaulas, agitándose por 
        los tíos que cuelgan de ellas.<br><br>
        Un chaval se me acerca, y me estira la mano mientras silba con la ayuda de dos dedos. 
        Estoy chorreando, y me muero de sed. Un recogevasos parece leerme el pensamiento, y 
        aparece con dos botellas de agua. Me las bajo del tirón, y continúo adelante: esto es 
        la guerra. Lanzo Magic Energy de Wax: bombo roto, sintes industriales y, de repente, 
        ese sonido terrorífico, como el del Vespino trucado de un afilador paranoico. Los tíos 
        golpean el suelo con las botas, marcando el ritmo del bombo; la bola de diez luces gira 
        sobre sus cabezas, quizás más rápida que nunca; la chapa que envuelve las columnas 
        parece a punto de despegarse. Y el afilador, percutiendo en mi cerebro.<br><br> 
        El éxtasis es generalizado. Querría meter algún Megabeat, pero ya no hay vuelta atrás. 
        Más madera. Coloco el nuevo disco, pero me equivoco de cara. Querría pinchar ambos 
        lados; pero no me quedará mucho tiempo, así que me decanto por mi preferido. Lo meto 
        rápido, y al instante la gente chilla al reconocerla: Tracy, de World Vol. 4. Me 
        pareció ver un lindo gatito… Intercambio, atenúo, enfatizo, corto. La luz en rojo. 
        Subo un fader, bajo el otro, y luego al revés. Miaaaaaaaaaaau... La pista es un 
        clamor...”.<br><br>
        New Beat: Bombos & Estrobos es la versión actualizada de Atticanos, también de 
        Pascal Ibiza.<br><br></p>

        <Hoverable let:hovering={hover}>
            <div>
            <button class:hover>
                {#if hover}
                <a target="_blank" href="https://amzn.to/2IqF0CI">
                    <Button> Tapa blanda </Button>
                </a>
                <a target="_blank" href="https://amzn.to/38AKZ2C">
                    <Button> ebook </Button>
                </a>
                {:else}
                    <Button>Comprar en Amazon</Button>
                {/if}
            </button>
            </div>
        </Hoverable> 
 
<style>
    .nb {
        border-radius: 5px;
        transition: width 0.1s, height 0.1s;
        display: block;
        margin: 0px auto;
    }
    @media screen and (max-width: 650px) {
    .nb {
        width: 70vw;
    }
    }
    @media screen and (min-width: 650px) {
    .nb {
        width: 70vw;
    }
    }
</style>