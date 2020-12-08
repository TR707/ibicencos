<script>
    import { createEventDispatcher } from 'svelte';
    import Button from "../shared/Button.svelte";
    import Hoverable from './Hoverable.svelte';
 </script>

<section>
    <h3 class="blue">2:42</h3><br>
    <img src="/img/242.jpg" alt="portada 2:42" class="dos"><br>
</section>
    <p>Una joven que sufre amnesia acaba de comenzar una relación con una misteriosa mujer. 
        Una noche recibe una extraña llamada, a las 2:42 AM.<br><br>
        A partir de ese momento, una serie de extraños incidentes, todos ellos relacionados con 
        su banda favorita, los belgas Front 242, convertirán su vida en una pesadilla...</p><br>
        <div class="container">
        <div class="center">
            <Hoverable let:hovering={hover}>
            <div>
                <button class:hover>
                    {#if hover}
                    <a target="_blank" href="https://amzn.to/32BGroT" class="conecta">
                        <Button> Tapa blanda </Button>
                    </a>
                    <a target="_blank" href="https://amzn.to/3naWvpi" class="conecta">
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
    .dos {
        border-radius: 5px;
        transition: width 0.1s, height 0.1s;
        display: block;
        margin: 0px auto;
        width: 200px;
    }
    .dos:hover {
        border-radius: 5px;
        transition: width 0.1s, height 0.1s;
        display: block;
        margin: 0px auto;
        width: 220px;
    }
    @media screen and (max-width: 650px) {
    .dos {
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
        