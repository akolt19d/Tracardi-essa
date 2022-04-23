<section class="container">
	<div class="smt">financial services</div>
	<div class="con">
		<div class="data">
			<p>obrazek</p>
			<p class="big">Make informed decisions with clean and compliant customer data</p>
			<p>
				Deliver personalized experiences at scale using complete, trustworthy, and compliant
				customer data.?
			</p>
			<button>Learn more about customer data</button>
		</div>
		<div class="code">
			<div>
				<div class="codetext">
					<p>Product view</p>
					<p class="secs">10s</p>
				</div>
				<h5>Collect</h5>
				<p class="normal">Personalize emails with recommendations based on user behavior.</p>
			</div>
			<div>
				<div class="codetext">
					<p class="added">Product added</p>
					<p class="secs">10s</p>
				</div>
				<h5>Understand</h5>
				<p class="normal">
					Identify traits of your high value customers and uncover key events along the customer
					journey that impact growth, engagement, and retention.
				</p>
			</div>
		</div>
	</div>
</section>

<style lang="scss">
	.container {
		@include vert;
		margin-top: 20vh;
		.smt {
			z-index: 1;
			width: 20%;
			margin: 100px 0;
			height: 9.5vh;
			color: $dark-blue;
			background-color: $dark-theme;
			box-shadow: 0px 4px 40px rgba(0, 0, 0, 0.25);
			border: 0;
			font-weight: bold;
			font-size: 20px;
			letter-spacing: 0.5px;
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			border-radius: 2px;
		}
		.con {
			width: 80%;
			display: flex;
			justify-content: space-around;
			.data {
				flex-basis: 35%;
				display: flex;
				flex-direction: column;
				align-items: center;
				.big {
					font-size: 28px;
					font-weight: 600;
				}
				p {
					margin: 70px 40px 30px 40px;
				}
				button {
					margin-top: 70px;
					width: 60%;
					height: 70px;
					font-weight: bold;
					text-decoration: underline;
					background-color: $yellow;
					border: none;
					box-shadow: 0px 4px 40px rgba(0, 0, 0, 0.25);
					border-radius: 2px;
					@include button-effects;
				}
			}
			.code {
				@include vert;
				justify-content: space-around;
				margin-top: 40px;
				flex-basis: 40%;
				div {
					flex-basis: 40%;
					display: flex;
					flex-direction: column;
					align-items: center;
					p {
						margin-top: 50px;
						width: 70%;
						text-align: center;
						font-size: 14px;
					}
					h5 {
						margin-top: 40px;
						font-size: 18px;
					}
					.codetext {
						background-color: $dark-theme;
						width: 360px;
						flex-basis: 50px;
						margin-top: 40px;
						display: flex;
						border-radius: 2px;
						justify-content: space-around;
						flex-direction: row;
						p {
							margin: 0 !important;
							color: $dark-blue;
						}
						.secs {
							color: grey;
						}
						.added {
							color: #ffc328;
						}
					}
				}
			}
		}
	}
</style>
