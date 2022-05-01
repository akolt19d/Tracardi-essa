<script>
	import Transition from '../svg/transition4.svelte';
</script>

<svg viewBox="0 0 1920 257" fill="none" xmlns="http://www.w3.org/2000/svg">
	<path
		d="M345.371 38.8608L0 12.7342V188H1929V86.7595C1911.9 70.7933 1875.67 38.8608 1867.54 38.8608C1859.42 38.8608 1672.61 26.4894 1575.94 0L1262.64 38.8608L748.135 86.7595L345.371 38.8608Z"
		fill="#1C1818"
	/>
	<g filter="url(#filter0_d_307_673)">
		<path
			d="M345.371 123.048L0 101.333V247H1929V162.857C1911.9 149.587 1875.67 123.048 1867.54 123.048C1859.42 123.048 1664.05 79.0159 1567.38 57L1262.64 123.048L748.135 162.857L345.371 123.048Z"
			fill="#1C1818"
		/>
	</g>
	<defs>
		<filter
			id="filter0_d_307_673"
			x="-30"
			y="7"
			width="1989"
			height="250"
			filterUnits="userSpaceOnUse"
			color-interpolation-filters="sRGB"
		>
			<feFlood flood-opacity="0" result="BackgroundImageFix" />
			<feColorMatrix
				in="SourceAlpha"
				type="matrix"
				values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
				result="hardAlpha"
			/>
			<feOffset dy="-20" />
			<feGaussianBlur stdDeviation="15" />
			<feComposite in2="hardAlpha" operator="out" />
			<feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.54 0" />
			<feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_307_673" />
			<feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_307_673" result="shape" />
		</filter>
	</defs>
</svg>
<footer>
	<div class="transition" />
	<div class="headline">
		<h3>TRACARDI</h3>
		<div>
			<input type="email" placeholder="Your work email" />
			<button> See how it works </button>
		</div>
	</div>
	<div class="contact">
		<div class="inner-wrapper">
			<ul class="ul-wrapper">
				<h5>ooomagad</h5>
				<li>'essa'</li>
				<li>'essa'</li>
				<li>'essa'</li>
			</ul>
			<ul class="ul-wrapper">
				<h5>ooomagad</h5>
				<li>'essa'</li>
				<li>'essa'</li>
				<li>'essa'</li>
			</ul>
			<ul class="ul-wrapper">
				<h5>ooomagad</h5>
				<li>'essa'</li>
				<li>'essa'</li>
				<li>'essa'</li>
			</ul>
		</div>
		<div>
			<h3>ooomagad</h3>
			<h6>essa</h6>
		</div>
	</div>
	<div class="end">
		<ul class="tos">
			<li>essa</li>
			<li>essa</li>
			<li>essa</li>
		</ul>
		<ul class="icons">
			<li>X</li>
			<li>X</li>
			<li>X</li>
			<li>X</li>
		</ul>
	</div>
</footer>

<style lang="scss">
	svg {
		width: 120%;
		margin-top: 40vh;
	}
	footer {
		font-size: 160%;
		margin-top: -4vh;
		color: $bg-l;
		background-color: $dark-theme;
		width: 100vw;
		padding: 3rem 8rem 8rem 8rem;
		padding-bottom: 3rem;
		position: relative;
		.transition {
			// position: absolute;
			// top: 0;
			// left: 0;
			width: 100%;
			height: 10vh;
		}
		.headline {
			margin: 5rem 0;
			display: flex;
			justify-content: space-between;
			h3 {
				font-size: 6rem;
			}
			input {
				outline: none;
				padding: 1.4rem 2rem;
				background: rgba($color: #fff, $alpha: 0.05);
				border: 0;
				border-radius: 1rem;
				text-align: center;
				transition: $theme-fade, 0.3s transform, 0.3s box-shadow;
				box-shadow: 0 0.2rem 0.6rem rgba($color: #000000, $alpha: 0.2);
				font-size: 80%;
				&::placeholder {
					font-weight: bold;
					color: rgba($color: #000000, $alpha: 0.55);
				}
			}
			button {
				padding: 1.4rem 2rem;
				background: 0;
				box-shadow: 0 0 0 0.05rem $yellow;
				border: 0;
				border-radius: 1rem;
				color: $bg-l;
				font-weight: bold;
				margin-left: 1rem;
				font-size: 80%;
				color: $yellow;
				transition: 0.3s background, 0.3s color, 0.3s transform, 0.3s box-shadow;
				cursor: pointer;
				&:hover,
				&:focus {
					box-shadow: 0 0 0 0.05rem #111;
					background: #111;
					color: white;
					transform: scale(0.97);
				}
				&:active {
					transform: scale(0.94);
				}
			}
		}
		.contact {
			margin: 4rem 0;
			display: flex;
			justify-content: space-between;
			.inner-wrapper {
				display: flex;
				justify-content: space-between;
				width: 50%;
				.ul-wrapper {
					list-style: none;
					* {
						margin: 3rem 0;
					}
				}
			}
		}
		.end {
			margin-top: 7rem;
			display: flex;
			justify-content: space-between;
			* {
				display: flex;
			}
		}
	}
</style>
