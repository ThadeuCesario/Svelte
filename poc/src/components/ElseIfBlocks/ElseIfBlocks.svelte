<script>
    let x = 11;
</script>

<div class="container">
    {#if x > 10}
        <p>{x} é maior que 10</p>
    {:else if x < 5}
        <p>5 é maior que {x}</p>
    {:else}
        <p>{x} está entre 5 e 10</p>
    {/if}
</div>

<style>
    .container {
        margin-top: 20px;
    }
</style>