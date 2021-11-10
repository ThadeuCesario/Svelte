<script>
    let count = 0;

    $: if(count > 9) {
            alert("Numero maximo atingido")
            count = 9;
        }

    function handleClick() {
        count += 1;
    }
</script>

<div>
    <button type="button" on:click={handleClick}>Incrementar</button>
    <strong>{count}</strong>
</div>