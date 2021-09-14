<script>
    let user = {
        loggedIn: false
    }

    function toggle() {
        user.loggedIn = !user.loggedIn;
    }
</script>

<div class="container">
    {#if user.loggedIn}
        <button type="button" on:click={toggle}>Logout</button>
    {/if}
    {#if !user.loggedIn}
        <button type="button" on:click={toggle}>Login</button>
    {/if}
</div>

<style>
    .container {
        margin-top: 20px;
    }
</style>