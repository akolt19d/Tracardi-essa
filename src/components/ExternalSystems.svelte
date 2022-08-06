<script>
	import Transition2 from './svg/transition2.svelte';
	import { fly } from 'svelte/transition';
	import { inview } from 'svelte-inview';
	let visible = false;
	let options = { rootMargin: '-100px' };
</script>

<section
	class="container"
	use:inview={options}
	on:enter={(event) => {
		visible = true;
	}}
>
	{#if visible}
		<div class="transition">
			<Transition2 />
		</div>
		<h2 in:fly={{ x: 1000, duration: 400, delay: 450 }} out:fly={{ duration: 300, delay: 1050 }}>
			INTERGRATE EXTERNAL <span class="white"> SYSTEMS</span>
		</h2>
		<div
			in:fly={{ x: -800, duration: 400, delay: 450 }}
			out:fly={{ duration: 400, delay: 1050 }}
			class="containerForContent"
		>
			<img class="obrazek" src="/popular.png" alt="ikonki popularnych firm" />
			<div class="conForText">
				<p class="fat">
					Use the <span class="blue">social media, SaaS, AI</span> to boost your sales. Integrate any
					system with your e-commerce solution.
				</p>
				<p class="small">
					Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has
					been the industry's standard dummy text ever since the 1500s,
				</p>
				<a href="/">Explore Tracardi for external systems.</a>
			</div>
		</div>
	{/if}
</section>

<style lang="scss">
	.container {
		width: 100%;
		//margin-top: 10vh;
		position: relative;
		.transition {
			height: 45vh;
			position: relative;
		}
		h2 {
			font-size: 4rem;
			text-align: center;
		}
		.containerForContent {
			display: flex;
			justify-content: center;
			align-items: center;
			width: 70vw;
			margin-left: 15vw;
			.conForText {
				display: flex;
				flex-basis: 30%;
				line-height: 140%;
				align-self: right;
				flex-direction: column;
				margin-top: 100px;
				text-align: justify;
				font-size: 18px;
				.small {
					color: grey;
					margin-bottom: 3.3rem;
				}
				.fat {
					font-weight: bold;
					margin-bottom: 3.3rem;
					.blue {
						color: $blue;
					}
				}
				a {
					color: $blue;
				}
			}
			.obrazek {
				margin: 100px 200px 20px 20px;
				width: 20vw;
				height: 20vw;
			}
		}
	}

	@media screen and (max-width: 800px) {
		.container {
			.transition {
				height: 15vh;
			}
			h2 {
				font-size: 220%;
			}
			.containerForContent {
				justify-content: center;
				flex-direction: column-reverse;
				align-items: center;
				.conForText {
					margin: 0 !important;
					max-width: 90%;
					width: 30rem;
					font-size: 100%;
				}
			}
		}
	}
</style>
