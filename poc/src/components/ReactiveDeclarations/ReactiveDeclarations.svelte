<script>
    let count = 1;

    //O '$' significa que executará novamente quando os valores mudarem
    $: dobro = count * 2;
    $: quadruplo = dobro * 2;

    function handleClick() {
        count += 1;
    }
</script> 

<div class="container">
    <button type="button" on:click={handleClick}>Contar</button>
    <strong>{count}</strong>
    <strong>{dobro}</strong>
    <strong>{quadruplo}</strong>
</div>

<style>
    .container {
        display: flex;
        align-items: center;
        justify-content: center;
        margin-top: 20px;
    }

    .container strong {
        margin: 0 20px;
    }
</style>