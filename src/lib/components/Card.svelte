<script>
	export let src, title, price, description
</script>
<div class="Card">
	<img {src} alt="Burguesas" class="Card__img">
	<div class="Card__title">
		<span class="Card__title-name">
			#{title}
		</span>
		<span class="Card__title-price">
			${price}
		</span>
	</div>
	<p class="Card__description">
		&nbsp;{description}
	</p>
</div>
<style>
	.Card{
		flex: 1 1 300px;
	}
	.Card__img{
		width: 100%;
		margin-bottom: 1rem;
	}
	.Card__title{
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-bottom: 1rem;
		color: #1b1b1b;
	}
	.Card__title-name{
		font-size: 1.3rem;
		text-transform: uppercase;
	}
	.Card__title-price{
		font-size: 1rem;
		font-weight: medium;
	}
	.Card__description{
		color: #5e5e5e;
		line-height: 1.4rem;
	}
</style>