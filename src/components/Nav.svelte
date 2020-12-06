<script context="module">

    import Libros from './Libros.svelte';
    import Tracklists from './Tracklists.svelte';
    import Subscribe from './Subscribe.svelte';
    import Relatos from './Relatos.svelte';
    
    export const navOptions = [
        { page: 'SUSCRÍBETE', component: Subscribe },
        { page: 'LIBROS', component: Libros },
        { page: 'TRACKLISTS', component: Tracklists },
        { page: 'RELATOS', component: Relatos },
            
    ];
    </script>