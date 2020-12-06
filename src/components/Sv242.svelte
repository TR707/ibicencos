<script>
    import { createEventDispatcher } from 'svelte';
    import Button from "../shared/Button.svelte";
    import Hoverable from './Hoverable.svelte';
 </script>

<section>
    <img src="/img/242.jpg" alt="portada 2:42" class="dos"><br>
    <h3 class="blue">2:42</h3><br>
</section>
    <p>Una joven que sufre amnesia acaba de comenzar una relación con una misteriosa mujer. 
        Una noche recibe una extraña llamada, a las 2:42 AM.<br><br>
        A partir de ese momento, una serie de extraños incidentes, todos ellos relacionados con 
        su banda favorita, los belgas Front 242, convertirán su vida en una pesadilla...<br><br>
        “Entonces sígueme el juego -dice mientras me coloca el antifaz-. Déjate llevar. 
        Sigue tus instintos.<br><br>
        Ya no puedo ver. Todo se ha vuelto oscuro.<br><br>
        -Y para hacerlo aún más interesante, voy a amordazarte. Es más divertido cuando 
        no puedes ver ni hablar, ¿verdad…?<br><br>
        Está esposándome con los brazos estirados hacia arriba, uno sobre cada madero.<br><br>
        -Y para terminar de crear la atmósfera perfecta, el toque final…<br><br>
        Escucho música viniendo desde mi derecha. Es Until Death (Us Do Part).<br><br>
        -Como podrás comprobar, he pensado en todo: tus queridos Front 242, para que la 
        experiencia sea aún mejor. Y ahora, voy a cambiarme de ropa. Estaré de vuelta antes 
        de que acabe la canción.<br><br>
        Por canción se refiere al enigmático Circling Overland (“1-1-2029…”), que suena más 
        terrorífico que nunca…"<br><br></p>
    
        <Hoverable let:hovering={hover}>
            <div>
            <button class:hover>
                {#if hover}
                <a target="_blank" href="https://amzn.to/32BGroT">
                    <Button> Tapa blanda </Button>
                </a>
                <a target="_blank" href="https://amzn.to/3naWvpi">
                    <Button> ebook </Button>
                </a>
                {:else}
                    <Button>Comprar en Amazon</Button>
                {/if}
            </button>
            </div>
        </Hoverable> 

<style>
    .dos {
        border-radius: 5px;
        transition: width 0.1s, height 0.1s;
        display: block;
        margin: 0px auto;
    }
    @media screen and (max-width: 650px) {
    .dos {
        width: 70vw;
    }
    }
    @media screen and (min-width: 650px) {
    .dos {
        width: 70vw;
    }
    }
</style>
        