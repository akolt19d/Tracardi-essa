<script>
	import { fly } from 'svelte/transition';
	import { inview } from 'svelte-inview';
	let visible = false;
	let options = { rootMargin: '-50px' };
</script>

<section
	use:inview={options}
	on:enter={(event) => {
		visible = true;
	}}
>
	{#if visible}
		<div
			class="nocode-wrapper"
			in:fly={{ opacity: 0, x: -1000, duration: 400, delay: 250 }}
			out:fly={{ opacity: 0, duration: 300, delay: 250 }}
		>
			<h3>NO CODE</h3>
			<p class="hei">NO CODE NO CODE</p>
			<p class="len">NO CODE NO CODE</p>
		</div>
		<div
			class="inner-wrapper"
			in:fly={{ opacity: 0, x: -1000, duration: 400, delay: 250 }}
			out:fly={{ opacity: 0, duration: 300, delay: 150 }}
		>
			<p class="developer">
				You <span style="color: black;"> don't have a developer</span> department, that's not a problem,
				integrate and run TRACARDI without writing any code.
			</p>
			<button class="btnDev">See how it works</button>
		</div>
		<img
			in:fly={{ opacity: 0, x: 1000, duration: 400, delay: 250 }}
			out:fly={{ opacity: 0, duration: 300, delay: 150 }}
			src="./noCodeMockup.png"
			alt="No Code Mockup"
		/>
	{/if}
</section>

<style lang="scss">
	section {
		background-color: $yellow;
		position: relative;
		// min-height: 60vh;
		img {
			position: absolute;
			top: 3rem;
			right: -1rem;
			width: 55%;
			max-width: 90%;
			filter: drop-shadow(0px 0px 10px rgba(black, 0.5));
		}
		.inner-wrapper {
			min-height: 30vh;
			// @include section-width;
			position: relative;
			left: 17.5%;
			top: 2vh;
			.developer {
				margin-top: 30px;
				width: 20%;
				text-align: justify;
				font-size: 20px;
				color: white;
				font-weight: bold;
			}
			.btnDev {
				width: 15rem;
				margin-top: 25px;
				height: 60px;
				background-color: black;
				border: none;
				color: white;
				font-weight: bold;
				cursor: pointer;
				transition: 0.2s;
				&:hover {
					color: black;
					background-color: white; //hover do zmiany narazie tylko poglądowo, dodatkowo przmieścić button bardziej do prawej
				}
			}
		}
		.nocode-wrapper {
			background-color: $yellow;
			width: 50%;
			height: 30rem;
			@include fc;
			justify-content: end;
			flex-direction: column;
			font-weight: bold;
			overflow: hidden;
			line-height: 2.5rem;
			padding: 2rem 0 0 2rem;
			//color: white;
			h3,
			p {
				background-image: linear-gradient(
					to right,
					white,
					white 55%,
					#111 55%,
					#111 80%,
					white 80%,
					$yellow 80%,
					$yellow 85%,
					white 85%
				);
				color: transparent;
				-webkit-background-clip: text;
				background-clip: text;
				background-size: 300% 100%;
				animation: 2.5s nocode alternate infinite linear;
			}
			h3 {
				font-size: 660%;
				@include fc;
				margin-left: 6rem;
				height: 6rem;
				animation-delay: 0.4s;
				animation-duration: 3s;
			}
			p {
				font-size: 270%;
				margin-left: -80px;
				font-weight: bold !important;
				&:first-of-type {
					transform: rotate(-90deg) translateY(1rem) translateX(-1rem);
					transform-origin: left;
				}
			}
			.len {
				width: 30rem;
			}
			.hei {
				margin-left: -185px;
				border-right: 3px solid white;
			}
		}
	}

	@keyframes nocode {
		0% {
			background-position: left;
		}
		100% {
			background-position: right;
		}
	}
</style>
