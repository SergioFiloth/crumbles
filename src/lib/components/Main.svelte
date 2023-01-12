<script>
    import Btn from '$lib/components/Btn.svelte';
</script>

<main class="Main">
    <h2 class="Main__title">
        Your day starts at Crumbles...
    </h2>
    <div class="Main--product">
        <div class="Main--product__img"/>
        <div class="Main--product-container">
            <span class="Main--product__title">
                Try our famous
            </span>
            <h3 class="Main--product__name">
                Cinnamon Rolls
                <div class="Btn--container">
                    <!-- <Btn text="Order Now" href="#" bgColor="#dd2c17"/> -->
                </div>
            </h3>
        </div>
    </div>
</main>
<style>
    .Main__title{
        background-color: #1a1a1a;
        padding: 1rem;
        text-align: center;
        font-size: 2rem;
        color: #fff;
        font-family: "Playball";
        font-weight: 400;
    }
    .Main--product{
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: repeat(2, 1fr);
        background-color: #f58d14;
    }
    .Main--product__img{
        background-image: url("/img/cinamons.png");
        background-size: cover;
        width: 100%;
        height: 100%;
    }
    .Main--product-container{
        padding: 2rem;
    }
    .Main--product__title{
        font-size: 2.5rem;
        font-style: italic;
    }
    .Main--product__name{
        font-family: Playball;
        font-size: 4.5rem;
        display: inline-block;
    }
    .Btn--container{
        margin-top: 1rem;
        width: 100%;
        display: flex;
        justify-content: flex-end;
        font-size: 1rem;
        font-family: "Roboto";
    }
    @media screen and (min-width: 768px) {
        .Main__title{
            font-size: 3.5rem;
            font-family: "Satisfy", sans-serif;
        }
        .Main--product{
            grid-template-columns: repeat(2, 1fr);
            grid-template-rows: 1fr;
        }
        .Main--product-container{
            padding: 6rem 2rem 7rem;
        }
    }
</style>