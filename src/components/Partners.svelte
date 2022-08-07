<script>
	import Transition5 from './svg/transition5.svelte';
	const partners = ['ibm', 'mac-os-logo', 'windows'];
	import { fly } from 'svelte/transition';
	import { inview } from 'svelte-inview';
	let visible = false;
	let options = { rootMargin: '-100px' };
</script>

<section>
	<div
		class="transition"
		use:inview={options}
		on:enter={(event) => {
			visible = true;
		}}
	>
		<Transition5 />
	</div>
	{#if visible}
		<div
			class="partner-opinion"
			in:fly={{ opacity: 0, x: -500, duration: 500, delay: 150 }}
			out:fly={{ opacity: 0, duration: 300, delay: 150 }}
		>
			<h3>IBM</h3>
			<div>
				<div>
					<p>
						Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea atque accusamus consequuntur
					</p>
					reiciendis nobis nostrum quo est dolores vero doloremque libero fugiat, aliquam veritatis sunt
					exercitationem eum consectetur, unde dignissimos.
				</div>
			</div>
			<div>
				<div>
					Lorem ipsum dolor, sit amet consectetur adipisicing elit. Impedit veniam ex voluptatum
					aperiam libero, blanditiis ratione suscipit qui mollitia corrupti quia maiores minima
					autem veritatis voluptate accusantium repellat? Voluptas, animi. voluptate
				</div>
			</div>
		</div>
	{/if}
	<ul
		class="partner-list"
		use:inview={options}
		on:enter={(event) => {
			visible = true;
		}}
	>
		{#each partners as partner, i}
			{#if visible}
				<li
					in:fly={{ y: 500, duration: 500, delay: i * 350 }}
					out:fly={{ duration: 300, delay: i * 250 }}
				>
					<img src="./{partner}.png" alt={partner} />
				</li>
			{/if}
		{/each}
	</ul>
</section>

<style lang="scss">
	section {
		min-height: 60vh;
		width: 100%;
		background-color: #1c1818;
		margin: 25vh 0 15vh 0;
		position: relative;
		padding-top: 5vh;
		.transition {
			width: 100%;
			height: 50px;
			position: absolute;
			top: 0;
		}
		.partner-opinion {
			width: 70rem;
			max-width: 90%;
			font-size: 5rem;
			text-align: center;
			height: 30rem;
			background-color: $yellow;
			margin: auto;
			justify-content: space-around;
			display: flex;
			align-items: center;
			div {
				flex-basis: 30%;
				margin: 20px;
				font-size: 19px;
				height: 70%;
				text-align: justify;
				p {
					color: white;
					margin-bottom: 20px;
					margin-top: 0;
					font-weight: bold;
				}
			}
			h3 {
				flex-basis: 25%;
			}
		}
		.partner-list {
			color: white;
			margin: 5rem auto;
			width: 30%;
			list-style-type: none;
			display: flex;
			justify-content: space-around;
			flex-direction: row;
			li {
				img {
					height: 6rem;
					filter: invert(100%);
					margin: 20px 20px 20px 60px;
					height: 80px;
				}
			}
		}
	}
</style>
