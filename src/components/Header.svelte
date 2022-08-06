<header>
	<h1>TRACARDI</h1>
	<p>
		Tracardi is an open-source <span class="blue">customer data platform</span> to help you engage your
		customers and build your sales through automated digital experiences.
	</p>
	<div>
		<!-- <h1>TRACARDI</h1> -->
		<input type="email" placeholder="Enter your email" />
		<button>Get Started</button>
	</div>
	<video autoplay muted loop src={`./webmzAlpha.webm`} />
</header>

<style lang="scss">
	header {
		position: relative;
		top: 12vh;
		min-height: 80vh;
		display: flex;
		flex-direction: column;
		align-items: center;
		// @include fc;
		@include section-width;
		text-align: center;
		// overflow-x: hidden;
		h1 {
			font-size: 400%;
			color: $blue;
			font-weight: 500;
		}
		div {
			z-index: 2;
			// position: absolute;
			// transform: translateY(-15vh);
			input {
				outline: none;
				padding: 0.8rem 1.8rem;
				background: darken($bg-l, 1);
				border: 0;
				border-radius: 0.125rem;
				box-shadow: -0.25rem -0.25rem 0.5rem white,
					0.25rem 0.25rem 0.5rem rgba($color: #000000, $alpha: 0.1);
				text-align: center;
				transition: $theme-fade, 0.3s transform, 0.3s box-shadow;
				&::placeholder {
					font-weight: bold;
				}
			}
			button {
				padding: 0.8rem 1.8rem;
				background: $orange;
				border: 0;
				border-radius: 0.125rem;
				color: $bg-l;
				font-weight: bold;
				box-shadow: -0.2rem -0.2rem 0.5rem white,
					0.2rem 0.2rem 0.5rem rgba($color: #000000, $alpha: 0.05);
				margin-left: 1rem;
				@include button-effects;
			}
		}
		video {
			position: absolute;
			top: 20vh;
			width: 70vw;
			margin: auto;
			// display: none;
		}
		p {
			z-index: 2;
			position: relative;
			// bottom: 10rem;
			font-size: 90%;
			font-weight: 500;
			// transform: translateY(-8vh);
		}
	}

	@media screen and (max-width: 600px) {
		header {
			video {
				display: none;
			}
		}
	}
</style>
