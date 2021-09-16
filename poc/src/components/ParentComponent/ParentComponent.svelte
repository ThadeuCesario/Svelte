<script>
    import ChildComponent from "../ChildComponent/ChildComponent.svelte";
    import OtherChildComponent from "../OtherChildComponent/OtherChildComponent.svelte";

    const data = {
        name: 'Thadeu Munhóz Cesário',
        age: 27,
        occupation: 'Software Developer',
        country: 'Brazil'
    }
</script>

<div class="container">
    <ChildComponent name="Parent props"/>
    <OtherChildComponent {...data} />
</div>

<style>
    .container {
        margin-top: 12px;
    }
</style>