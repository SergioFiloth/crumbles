<script>
	import Card from "$lib/components/Card.svelte"

	let products = [
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/SINGLE_1_g5f9ev.jpg",
            title: "Single",
            price: "1.65",
            description: "Butter biscuit"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/LONELY_1_lgycje.jpg",
            title: "Lonely",
            price: "2.65",
            description: "Egg and Cheese"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/ROOMMATE_1_cs4kr1.jpg",
            title: "Roommate",
            price: "3.95",
            description: "Bacon and Cheese"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/PORKY_1_bbgxa7.jpg",
            title: "Porky",
            price: "2.95",
            description: "Sausage"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/GM_1_elschv.jpg",
            title: "GM",
            price: "3.95",
            description: "Sausage, Egg and Cheese"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/NICE_1_hdk8g7.jpg",
            title: "Nice",
            price: "4.95",
            description: "Bacon, Egg and Cheese"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217741/crumbles/breakfast/DGB_1_islpuo.jpg",
            title: "DGB",
            price: "4.95",
            description: "Double Sausage, Bacon, Egg and Cheese"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/Angry_Chick_1_s5bx07.jpg",
            title: "Angry Chick",
            price: "4.95",
            description: "Chicken"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217740/crumbles/breakfast/COUNTRY_1_rflsyx.jpg",
            title: "Country",
            price: "4.95",
            description: "Steak and Egg"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649217741/crumbles/breakfast/STRIPPERS_1_gou4ou.jpg",
            title: "Strippers",
            price: "4.95",
            description: "Triple Bacon and Cheese"
		},
		{
			src: "https://res.cloudinary.com/dnhffenno/image/upload/v1649977247/crumbles/breakfast/Hammer_wtbz3q.png",
            title: "Hammer",
            price: "4.95",
            description: "Ham and American Cheese"
		}
	]
</script>
<main class="Main">
	<div class="Main--principal">
		<a href="/" sveltekit:prefetch class="Main--principal__link">
			<img src="/img/logo.png" alt="Logo" class="Main--principal__logo">
		</a>
		<h2 class="Main--principal__title">
			Our Menu
		</h2>
	</div>
	<div class="Main--container">
		<h3 class="Main--title">Breakfast</h3>
		<!-- <p class="Main--subtitle">
			All burgers served with waffle fries
		</p> -->
		<div class="Main--content-card">
			{#each products as product}
				<Card 
					src={product.src}
					title={product.title}
					price={product.price}
					description={product.description}
					/>
			{/each}
		</div>
	</div>
	<!-- <div class="hr"></div>
	<p class="Main--subtitle-bottom">
		Breakfast Served Daily 7am-11am (Sunday 8am)
	</p> -->
</main>
<style>
	.Main{
		padding: 2rem 1rem 2rem;
		text-align: center;
	}
	.Main--principal{
		position: sticky;
		top: 0;
		left: 0;
		background-color: #fff;
		padding: 1rem;
	}
	.Main--principal__link{
		height: 100%;
		position: absolute;
		top: 0;
		left: 0;
		display: flex;
		align-items: center;
	}
	.Main--principal__logo{
		height: 70%;
		transition: height .3s;
	}
	@media (hover: hover) {
		.Main--principal__logo:hover{
			height: 90%;
		}
	}
	.Main--principal__title{
		text-transform: uppercase;
		font-size: 2.4rem;
		margin-bottom: .5rem;
		color: var(--principal);
		font-family: sans-serif;
	}
	.Main--container{
		margin-bottom: 1rem;
		padding-bottom: 1.25em;
	}
	.Main--title{
		margin-top: 1.25rem;
		font-size: 2rem;
		color: var(--principal);
		font-weight: 400;
		margin-bottom: 0.3rem;
		margin-bottom: 2rem;
	}
	.Main--subtitle{
		color: #595959;
		font-size: 0.9rem;
		margin-bottom: 5rem;
		line-height: 2,5rem;
	}
	.Main--content-card{
		display: grid;
        grid-template-columns: repeat(1, 1fr);
		justify-content: center;
		gap: 4rem;
		flex-wrap: wrap;
		text-align: left;
	}
	.Main--subtitle-bottom{
		color: #595959;
		font-size: 0.9rem;
		margin-bottom: 5rem;
		line-height: 2,5rem;
		margin-bottom: 0;
		margin-top: 6rem;
	}
	@media screen and (min-width: 480px) {
		.Main{
			padding: 4rem 2rem 2rem;
		}
	}
	@media screen and (min-width: 768px) {
		.Main{
			padding: 2rem 8rem 2rem;
		}
		.Main--principal__logo{
			height: 100%;
		}
		@media (hover: hover) {
			.Main--principal__logo:hover{
				height: 120%;
			}
		}
		.Main--content-card{
			grid-template-columns: repeat(3, 1fr);
		}
	}
</style>