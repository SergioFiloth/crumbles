<script>
    import Btn from "$lib/components/Btn.svelte"
</script>
<div class="Hero">
    <div class="Hero--presentation">
        <img src="/img/logo.png" alt="Logo" class="Hero--presentation__img">
        <div class="Hero--presentation-text-container">
            <h2 class="Hero--presentation__title">
                Breakfast
            </h2>
            <span class="Hero--presentation__description">
                Home baked Biscuits
            </span>
            <!-- <Btn text="Order Now" href="#" bgColor="#dd2c17"/> -->
        </div>
    </div>
    <div class="Hero--img">
        <img src="/img/biscuit.png" alt="Biscuits" class="Hero--img__img">
    </div>
</div>
<style>
    .Hero{
        display: grid;
    }
    
    .Hero--presentation{
        display: flex;
        flex-direction: column;
        color: var(--secundary-text)
    }
    .Hero--presentation__img{
        max-width: 250px;
        margin-top: -4.5rem;
        margin-bottom: 2.5rem;
    }
    .Hero--presentation__title{
        font-style: italic;
        font-size: 2.5rem;
    }
    .Hero--presentation__description{
        font-size: 4rem;
        font-family: "Playball", cursive;
        font-weight: 600;
        display: block;
        margin-bottom: 1rem;
    }
    img{
        max-width: 50%;
    }
    .Hero--img{
        display: grid;
        justify-content: center;
    }
    .Hero--img__img{
        margin: 2rem auto;
    }
    @media screen and (min-width: 768px) {
        .Hero{
            display: flex;
            justify-content: space-between;
        }
        .Hero--img{
            display: initial;
        }
        img{
            max-width: 100%;
        }
    }
</style>