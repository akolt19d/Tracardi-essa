<section class="container">
	<h2>Use Tracardi to integrate with best-in-class tools</h2>
	<p>
		Enable the best product analytics tools, A/B testing tools, and data warehousing tools with the
		flip of a switch.
	</p>
	<img src="./sexo.png" alt="options" />
	<button>Explore</button>
</section>

<style lang="scss">
	.container {
		margin-top: 35vh;
		@include vert;
		h2 {
			z-index: 1;
			color: $different-blue;
			font-size: 50px;
			width: 50%;
			text-align: center;
		}
		p {
			opacity: 0.5;
			margin-top: 50px;
			font-size: 20px;
			width: 50%;
			text-align: center;
			z-index: 1;
			margin-bottom: 5rem;
		}
		img {
			width: 40%;
			filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
		}
		button {
			background-color: #3779ef;
			width: 16vw;
			height: 7.5vh;
			border-radius: 2px;
			border: none;
			font-size: 25px;
			color: white;
			font-weight: 600;
			margin-top: 10vh;
			@include button-effects;
			position: relative;
			&::after {
				position: absolute;
				width: 16vw;
				height: 7.5vh;
				background-color: red;
				margin-top: 0%;
				margin-left: -60%;
				z-index: -1;
				background-color: $dark-theme;
				content: '';
			}
			&:hover::after {
				background-color: transparent;
			}
			&:active::after {
				background-color: transparent;
			}
			&:focus::after {
				background-color: transparent;
			}
		}
	}
</style>
