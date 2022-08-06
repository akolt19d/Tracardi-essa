<script>
	import Transition from './svg/transition3.svelte';
	import { fly } from 'svelte/transition';
	import { inview } from 'svelte-inview';
	let cats = [
		{
			id: 1,
			name: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio
				quas repellendus dicta voluptas recusandae quod!`
		},
		{
			id: 2,
			name: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio
				quas repellendus dicta voluptas recusandae quod!`
		},
		{
			id: 3,
			name: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio
				quas repellendus dicta voluptas recusandae quod!`
		},
		{
			id: 4,
			name: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio
				quas repellendus dicta voluptas recusandae quod!`
		},
		{
			id: 5,
			name: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio
				quas repellendus dicta voluptas recusandae quod!`
		},
		{
			id: 6,
			name: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio
				quas repellendus dicta voluptas recusandae quod!`
		}
	];
	let visible = false;
	let isInView;
	const options = {};
</script>

<section class="container">
	<div class="transition">
		<Transition />
	</div>
	<div
		class="conForData"
		use:inview={options}
		on:enter={(event) => {
			visible = true;
		}}
	>
		{#each cats as { id, name }, i}
			{#if visible}
				<div
					in:fly={{ y: -500, duration: 500, delay: i * 150 }}
					out:fly={{ duration: 300, delay: i * 150 }}
				>
					{i + 1}.{name}
				</div>
			{/if}
		{/each}
	</div>
</section>

<style lang="scss">
	.container {
		width: 100%;
		background: #3b78ed;
		min-height: 80vh;
		margin-top: 12rem;
		padding: 5rem 0;
		position: relative;
		background-color: $blue;
		color: white;
		.transition {
			position: absolute;
			left: 0;
			top: 0;
			background: white;
			width: 100%;
			height: 24vh;
		}
		.conForData {
			display: flex;
			width: 70%;
			min-height: 60vh;
			margin: 3rem 15%;
			flex-wrap: wrap;
			justify-content: center;
			overflow-x: hidden;
			//@include fc;
			gap: 3rem 1.75rem;
			div {
				flex-basis: 31%;
				height: 35vh;
				svg {
					margin-bottom: 20px;
				}
				//margin: 5rem 0;
				background-color: #111;
				padding: 20px;
				align-items: center;
				display: flex;
				aspect-ratio: 1.2/1;
				flex-direction: column;
				z-index: 1;
				h2 {
					margin-top: 2vh;
				}
				p {
					margin-top: 5vh;
					width: 70%;
					text-align: justify;
					color: $yellow;
				}
			}
		}
	}
</style>
