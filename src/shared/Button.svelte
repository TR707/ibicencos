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
        border: 0;
        cursor: pointer;
        border-radius: 6px;
        padding: 8px 8px;
        box-shadow: 1px 2px 3px white;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: -10px;
        margin-left: -10px;
        margin-top: -4px;
        margin-bottom: -4px;
        width: 170px;  
    } 
    button:link {
        text-decoration: none;   
    }
    .primary, .secondary, .primary.inverse, .secondary.inverse  {
        border: 2px solid black;
    }
    .primary, .secondary {
        background: gold;
        color: black;
    }
    .primary {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .secondary {
        font-family: 'Share Tech Mono', -apple-system, BlinkMacSystemFont, "Segoe UI", 
                      Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;   
    }
    .flat{
        box-shadow:none;
        background-color: white;
        background: gold;
    }
    .primary.inverse, .secondary.inverse {
        color: gold;
        background: black;
    }

    button:hover {
        text-decoration: none;   
    }
</style>
