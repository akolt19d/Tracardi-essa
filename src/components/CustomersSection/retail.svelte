<section class="container">
	<button>retail</button>
	<div class="conForContent">
		<div class="sendMail">
			<p class="big">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores dolorem possimus
				eligendi laborum facilis earum perferendis dolore esse sapiente? Repellendus.
			</p>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores dolorem possimus
				eligendi laborum facilis earum perferendis dolore esse sapiente? Repellendus.
			</p>
			<div>
				<input type="text" placeholder="your email..." />
				<button>Get started</button>
			</div>
		</div>

		<div class="code">
			<div>
				<div><p>lorem</p></div>
				<div><p>lorem</p></div>
				<div><p>lorem</p></div>
			</div>
			<p>Learn more about events</p>
		</div>
	</div>
</section>

<style lang="scss">
	.container {
		margin-top: 30vh;
		background-color: black;
		@include vert;
		button {
			width: 20%;
			margin: 100px 0;
			height: 9.5vh;
			color: black;
			background-color: $light-blue;
			border-radius: 2px;
			border: 0;
			font-weight: bold;
			font-size: 20px;
			letter-spacing: 0.5px;
			cursor: pointer;
			@include button-effects;
		}
		.conForContent {
			color: white;
			display: flex;

			width: 80%;
			justify-content: space-around;
			.sendMail {
				display: flex;
				flex-basis: 35%;

				flex-direction: column;
				align-items: center;
				p {
					margin: 40px 20px 20px 20px;
					text-align: left;
				}
				.big {
					font-size: 18px;
					font-weight: 500;
				}
				div {
					width: 100%;
					display: flex;
					justify-content: space-around;
					align-items: center;
					button {
						flex-basis: 29%;
						height: 7vh;
						margin-left: -80px;
					}
					input {
						flex-basis: 40%;
						height: 50px;
						height: 7vh;
						margin-left: -20px;
						font-size: 15px;
						text-align: center;
					}
				}
			}
			.code {
				flex-basis: 45%;
				@include vert;
				justify-content: center;

				div {
					background-color: white;
					flex-basis: 60%;
					width: 70%;
					display: flex;
					border-radius: 2px;
					flex-direction: column;
					justify-content: center;
					align-items: center;
					div {
						width: 80%;
						flex-basis: 25%;
						display: flex;
						justify-content: center;
						margin: 0;
						p {
							background-color: black;
							width: 100% !important;
							color: orange;
							border-radius: 2px;
							text-align: left;
							padding: 20px;
						}
					}
				}
				p {
					margin-top: 20px;
					color: #3081ff;
					font-weight: 600;
					text-decoration: underline;
				}
			}
		}
	}
</style>
