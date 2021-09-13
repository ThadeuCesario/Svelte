<script>
    let user = {
        loggedIn: false
    }

    function toggle() {
        user.loggedIn = !user.loggedIn
    }
</script>

<div class="container">
    <strong>Using else block</strong>
    {#if user.loggedIn}
        <button type="button" on:click={toggle}>Logout</button>
    {:else}
        <button type="button" on:click={toggle}>Login</button>
    {/if}
</div>

<style>
    .container {
        margin-top: 20px 0 0 0;
    }
</style>