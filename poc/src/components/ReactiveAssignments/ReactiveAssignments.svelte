<script>
    let count = 0;
    
    function handleClick() {
        count += 1;
    }
</script>

<div class="container">
    <button on:click={handleClick}>
        Somar
    </button>
    <span>{count}</span>
</div>

<style>
    .container {
        margin: 15px 0 0 0;
    }
</style>
