<script>
    import { createEventDispatcher } from 'svelte';
    import Button from "../shared/Button.svelte";
    import Hoverable from './Hoverable.svelte';
 </script>

<section><br>
    <h3 class="blue">Techno Camina Conmigo:<br>Bandas y productores que lideraron 
        la electrónica nacional (89-93)</h3><br>
    <img src="/img/Techno Camina Conmigo.jpg" alt="portada Techno Camina Conmigo" class="tecece"><br>
</section>        
        <p>Durante la segunda década de los 80, Valencia se ha convertido en una de las 
        capitales europeas de la vanguardia musical por su atractiva combinación de 
        sonidos sintéticos y guitarreros.<br><br>
        A partir de 1989, unos cuantos artistas nacionales se lanzarán a crear sonidos 
        avanzados, que acabarán con el monopolio de la electrónica foránea en las pistas 
        de baile y que contribuirán a crear la banda sonora de aquella irrepetible 
        época.<br><br>
        <b>Germán Bou</b><br>
        “Las olas del mar, los cantos de los monjes y las campanas parecen transportarte 
        a otra época (…) Germán ha encontrado un santo grial (…) Así Me Gusta A Mí arde
        con las cuerdas y los dramáticos coros sobre los que planean un puñado de efectos 
        extraterrestres (...) El calor y la tensión se vuelven insoportables, y todo acaba 
        convertido en magma. La lava sale disparada, y aterriza sobre la pista en forma de 
        terrible secuencia EBM...”<br><br>
        <b>Dimas & Martinez</b><br> 
        “Que Idea! es una combinación explosiva: ritmos cuadriculados y acero, cuerdas 
        de violín y samples vocales. Fuerza e imaginación. Ritmos maquinales y chulería 
        italo disco. Disciplina y hedonismo (…) La remezcla juguetea con el gancho original, 
        cortándolo y reordenándolo, y repitiéndolo compulsivamente hasta que el track se 
        convierte en una máquina enloquecida...”<br><br>
        <b>Flash Zero</b><br>
        “Las canciones han muerto, ¿dónde están? Han sido reemplazadas por tracks, cortes 
        sin estructura, repetitivos, hipnotizantes (…) Las baterías electrónicas tocadas 
        en directo aportan un groove imposible de lograr con cajas de ritmos”.<br><br>
        <b>Megabeat</b><br>
        “Next Light escupe voces robóticas y rugidos industriales, y las percusiones 
        metálicas de Nexus 6 parecen tocadas por androides de última generación (…) A 
        Picture Of You, un track bellísimo en el que la emoción alcanza niveles 
        máximos”.<br><br>
        <b>Nacho Division</b><br>
        “Albades Muro suena incandescente, radiactivo, desintegrador. Pitidos que atacan 
        el sistema nervioso, saturación, luces en rojo. Avalanchas metálicas, ruido, 
        paranoia… ¿Es la aguja la que hace sonar el vinilo, o son mis uñas al rascarlo? (…) 
        El arranque como productor de Nacho Division ha sido devastador, ¿volveremos algún 
        día a ver la luz del sol…?”<br><br>
        Techno Camina Conmigo repasa los discos con la ayuda de sus creadores, e incluye 
        entrevistas exclusivas a Chus del Gallego <b>(Berlin)</b> + Xema Sentí <b>(Binari)</b> 
        + Dimas Carbajo <b>(Dimas & Martinez)</b> + Fan Dl Kaox <b>(Flash Zero)</b> 
        + Germán Bou <b>(Espiral, Boa Club, Toss)</b> + Jota Demasiado <b>
        (J & Zona Industrial) </b> + Juanjo Aranda <b>(J.J. Fax) </b> 
        + Juan Laforga <b>(Ritual, 666 Frecuencia)</b> + Juanjo Bosque <b>(KRB)</b> + 
        Fran Lenaers <b>(Megabeat)</b> + Nacho Division + Roger Muñoz <b>(Teknika) </b> + 
        Salvador Aleixandre <b>(Último Destino, Teube)</b> + Víctor Tomé <b>(Ut Supra).</b><br><br>
        Qué máquinas utilizan, qué sienten al alcanzar el éxito, cómo lo gestionan y cómo 
        acaban reinventándose como artistas.<br><br>
        «Necesito experimentar algo fuera de lo cotidiano: sentir placer, sumergirme en la 
        inquietud, flotar en relax total. Sin esto, no hay un producto musical 
        ilusionante...» <b>(Germán Bou)</b>.<br><br>
        «Los temas por acabar están en mi cabeza, a la espera, hasta que por fin un día veo 
        cómo expresarlos (…). Entonces escribo esa idea, y sale del tirón, porque ya sé el 
        qué y cómo expresarlo. Ese momento es de una sensación orgásmica...» <b>(Fan DI Kaox)</b>.<br><br>
        «Le explico mis inquietudes con su obra y le presento la mezcla entre su Maximizing y 
        The Ride Inside. Cuál es mi sorpresa cuando Wim, una persona tremendamente educada, 
        me dice que ya la conoce…» <b>(Juan Laforga aka Ritual)</b>.<br><br>
        «Un DJ es un educador, y también un psicólogo. Porque la sesión hay que trabajarla con 
        mucha psicología, controlando las sensaciones que la gente expresa en la 
        pista…» <b>(Nacho Division aka Mirage Of Deep)</b></p>.
        <div class="container">
        <div class="center">
            <Hoverable let:hovering={hover}>
                <div>
                <button class:hover>
                    {#if hover}
                    <a target="_blank" href="https://amzn.to/36ux9Mn" class="conecta">
                    <Button> Tapa blanda </Button>
                    </a>
                    <a target="_blank" href="https://amzn.to/3pmcnHp" class="conecta">
                        <Button> ebook </Button>
                    </a>
                    {:else}
                        <Button>Comprar en Amazon</Button>
                    {/if}
                </button>
                </div>
            </Hoverable>
    </div>
    </div>
<style>
    .tecece {
        border-radius: 5px;
        transition: width 0.1s, height 0.1s;
        display: block;
        margin: 0px auto;
        width: 200px;
    }
    .tecece:hover {
        border-radius: 5px;
        transition: width 0.1s, height 0.1s;
        display: block;
        margin: 0px auto;
        width: 220px;
    }
    @media screen and (max-width: 650px) {
    .tecece {
        width: 70vw;
    }
    }
    .center {
	margin: 0;
	position: absolute;
	left: 50%;
	-ms-transform: translate(-50%, -50%);
	transform: translate(-50%, -50%);
  }
</style>
                