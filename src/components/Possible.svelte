<script>
	import { fly } from 'svelte/transition';
	import { inview } from 'svelte-inview';
	let Posibilites = [
		{
			title: 'How Tracardi works?',
			element: `Tracardi collects events that happen across multiple channels. Then
			is sends them to a visual editor where you can process it, orchestrate to other systems such as
			AI product referral systems, or interact with the user directly via micro front-ends`
		},
		{
			title: 'How much does it costs?',
			element: `It is up to you. TRACARDI is a  free softwareas long as you install
			it on premises and maintain it yourself. For cloud solutions please contact us.`
		},
		{
			title: 'Can i intergrate it on my old school web page?',
			element: `Sure. Integration is as simple as pasting a JavaScript code.`
		}
	];
	let visible = false;
	let options = {};
</script>

<section class="container">
	<h2>How is this all possible</h2>
	<div
		class="containerForCon"
		use:inview={options}
		on:enter={(event) => {
			visible = true;
		}}
	>
		{#each Posibilites as { title, element }, i}
			{#if visible}
				<h2
					in:fly={{ opacity: 0, x: -500, duration: 500, delay: i * 150 }}
					out:fly={{ opacity: 0, duration: 300, delay: i * 150 }}
				>
					{title}
				</h2>
				<p
					in:fly={{ x: -500, duration: 500, delay: i * 150 }}
					out:fly={{ duration: 300, delay: i * 150 }}
				>
					{element}
				</p>
			{/if}
		{/each}
	</div>
	<button class="yellowButoonQuest">I have more questions!</button>
</section>

<style lang="scss">
	.container {
		width: 100%;
		@include fc;
		flex-direction: column;
		overflow-x: hidden;
		h2 {
			text-align: center;
			font-size: 3rem;
			font-weight: bold;
		}
		.containerForCon {
			display: flex;
			flex-direction: column;
			margin-top: 10vh;
			width: 40%;
			transform: translateX(10rem);
			p {
				margin-top: 5vh;
				text-align: left;
				line-height: 150%;
			}
			h2 {
				text-align: left;
				font-size: 2.2rem;
				margin-top: 10vh;
				position: relative;
				&:first-child {
					margin-top: 2vh;
					&::before {
						background-color: #111;
					}
				}
				&::before {
					content: '';
					position: absolute;
					left: -10rem;
					top: -1rem;
					height: 5rem;
					aspect-ratio: 1/1;
					background-color: $blue;
					border-radius: 10px;
					box-shadow: 0 0 10px 0 rgba(black, 0.5);
				}
				&:last-of-type {
					&::before {
						background-color: $yellow;
					}
				}
			}
			.szer {
				width: 120%;
			}
			.free {
				color: $blue;
			}
		}
		.yellowButoonQuest {
			margin-top: 15vh;
			width: 220px;
			height: 60px;
			margin-left: 25vw;
			border: none;
			background-color: $yellow;
			cursor: pointer;
			font-size: 15px;
			font-weight: bold;
		}
	}

	@media screen and (max-width: 800px) {
		.container {
			.containerForCon {
				width: 90%;
				margin: 0;
			}
		}
	}
</style>
