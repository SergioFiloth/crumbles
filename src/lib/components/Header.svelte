<script>
    import Btn from "$lib/components/Btn.svelte"
</script>
<header class="Header">
    <Btn text="Menu" href="/menu" bgColor="#000000"/>
</header>
<style>
    .Header{
        background-color: var(--principal);
        padding: 1rem;
        display: flex;
        justify-content: flex-end;
    }
</style>