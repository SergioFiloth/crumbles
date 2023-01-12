<div class="Footer">
    <img src="/img/logo.png" alt="" class="Footer__logo">
    <div class="Footer--seccion">
        <div class="Footer__title">Crumbles</div>
        <div class="Footer--text">
            <div class="Footer__text">Menu</div>
            <div class="Footer__text">Contact us</div>
        </div>
        <a href="https://www.instagram.com/crumblesstore/" target="_blank">
            <img src="/img/icons/instagram.svg" alt="Social SVG">
        </a>
        <a href="https://www.facebook.com/crumblesonkirk" target="_blank">
            <img src="/img/icons/facebook.svg" alt="Social SVG">
        </a>
    </div>
    <div class="Footer--seccion">
        <div class="Footer__title">Crumbles</div>
        <div class="Footer--text">
            <div class="Footer__text">Your morning starts here at Crumbles! Crumbles is a small humble place where you can get your Biscuit. Cinnamon Rolls & Coffee made fresh! Rise & Grind every morning with us!</div>
        </div>
    </div>
</div>
<style>
    .Footer{
        background-color: #000;
        color: #fff;
        display: grid;
        grid-template-columns: 1fr;
        gap: 2rem;
        padding: 2rem;
    }
    .Footer > *{
        width: 100%;
    }
    .Footer__logo{
        width: 75%;
        margin: 0 auto;
    }
    .Footer__title{
        color: #fdd225;
        font-size: 1.2rem;
        margin-bottom: .5rem;
    }
    .Footer--text{
        margin-bottom: 1rem;
    }
    @media screen and (min-width: 768px) {
        .Footer{
            grid-template-columns: 30% 2fr 4fr;
        }
        .Footer__logo{
            width: 50%;
            margin-left: 2rem;
        }
    }
</style>