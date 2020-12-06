<script>
    export let type = 'primary';
    export let flat = false;
    export let inverse = false;
</script>

<button class={type} class:flat={flat} class:inverse={inverse} on:click>
    <slot></slot>    
</button>

<style>
    button {
        border:0;
        cursor: pointer;
        border-radius: 6px;
        padding: 8px 8px;
        font-weight:bold;
        box-shadow: 1px 2px 3px rgba(0,0,0,0.2);

    } 
    .primary {
        background: gold;
        color: black;
        border: 2px solid black;
    }
    .secondary {
        background: gold;
        color: black;
        border: 2px solid black;
        font-family: 'Share Tech Mono', -apple-system, BlinkMacSystemFont, "Segoe UI", 
                      Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;  
    }
    .flat{
        box-shadow:none;
        background-color: #f5f5f5;
        background: gold;
    }
    .primary.inverse {
        color: gold;
        background: black;
        border: 2px solid black;
    }
    .secondary.inverse {
        color: gold;
        background: black;
        border: 2px solid black;
    }
    .slot {
        background-color: #f5f5f5;
    }
</style>