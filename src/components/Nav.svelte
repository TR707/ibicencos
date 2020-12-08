<script context="module">

    import Libros from './Libros.svelte';
    import MRWhiteLabel from './MRWhiteLabel.svelte';
    import Subscribe from './Subscribe.svelte';
    import Tracklists from './Tracklists.svelte';
    
    export const navOptions = [
        { page: 'LIBROS', component: Libros },
        { page: 'MR WHITE LABEL', component: MRWhiteLabel }, 
        { page: 'SUSCRÍBETE', component: Subscribe },
        { page: 'TRACKLISTS', component: Tracklists },
    ];
    </script>