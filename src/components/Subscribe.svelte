<script>  
    import { createEventDispatcher } from 'svelte';
    import Button from "../shared/Button.svelte";
    let fields = { email: ''};
    let errors = { email: ''};
    let valid = false;
    let dispatch = createEventDispatcher(); 
    const subscribeURL = 'http://localhost:3000/subscribe/';

   const verificaFormatoEmail = () => {
       var regexp = new RegExp(/^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/)
        if ( ! regexp.test(fields.email)) {
            valid = false;
            errors.email ='introduzca un formato correcto';
        } else {
            errors.email ='';
            valid = true;
        }
    }  
    function enviar () {
        if (valid) {
            console.log('Enviando')
    
            var data = new FormData();
            data.append('email',fields.email);
    
            var requestOptions = {
                method: 'POST',
                body: data,
            };
            fetch(subscribeURL,requestOptions)
            .then(res=>window.alert('¡Gracias por suscribirte!'))
            .catch(res=>window.alert('Algo salió mal'))
            ;
        } else {
            errors.email = 'Formato incorrecto'
        }
    }
</script>

<div class="row">
    <div class="col s12">
        <div class="row"><br>
            <p>¿Quieres saber qué estoy tramando? 
                Suscríbete y serás el primero en saberlo...</p>
            <form on:submit|preventDefault={enviar}><br> 
                <div class="form-field">
                    <label for="email"></label>
                    <input on:keyup={verificaFormatoEmail} type="text" placeholder="email" id="email" bind:value="{fields.email}">
                    <div class="error">{ errors.email }</div>
                </div>
                    <Button type="secondary" flat={true} >Enviar</Button>   
            </form>
        </div>
    </div>
</div>           
    
<style>
    form{
        width: 100%;
        margin: 0 auto;
        text-align: center;     
        color: black;  
    }
    .form-field{
        margin: 18px auto;     
    }
    input{
        width: 90%;
        height: 25%;
        border-radius:6px; 
        font-family: 'Share Tech Mono', -apple-system, BlinkMacSystemFont, "Segoe UI", 
	             Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;
	    font-size: 4.5vw;  
    }
    label{
        margin: 10px auto;
        text-align:left;
        color: black;
    }
    .error{
        font-weight: bold;
        color: #d91b42;
        font-family: 'Share Tech Mono', -apple-system, BlinkMacSystemFont, "Segoe UI", 
	             Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;
	    font-size: 4.5vw;
    }  
</style>