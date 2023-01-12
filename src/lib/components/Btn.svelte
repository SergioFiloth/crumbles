<script>
    export let text, href, bgColor
</script>
<a {href} sveltekit:prefetch style="background-color: {bgColor}" class="Btn">{text}</a>

<style>
    .Btn{
        padding: .75rem 0.5rem;
        border-radius: 5px;
        color: #fff;
        cursor: pointer;
        display: inline-block;
    }
</style>