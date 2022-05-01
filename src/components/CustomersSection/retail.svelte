<svg viewBox="0 0 1920 1331" fill="none" xmlns="http://www.w3.org/2000/svg">
	<g filter="url(#filter0_d_433_85)">
		<path
			d="M818.203 158.957L343.952 89.2432L-10.7132 132.67L-10.9432 452.054L-11.0335 574.043L1944.6 572.737L1945 30L1686.38 88.3693L1381.53 158.591L818.203 158.957Z"
			fill="#0094FF"
		/>
	</g>
	<g filter="url(#filter1_d_433_85)">
		<path
			d="M709.864 201.346L305.208 146.438L-21.2075 184.123L-9.85153 1018.55L-8.84279 1302.45L1944.92 1317.03L1940.43 53.9625L1684.59 119.544L1361.21 215.449L709.864 201.346Z"
			fill="#1C1818"
		/>
	</g>
	<defs>
		<filter
			id="filter0_d_433_85"
			x="-31.0334"
			y="0"
			width="1996.03"
			height="584.043"
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
			<feOffset dy="-10" />
			<feGaussianBlur stdDeviation="10" />
			<feComposite in2="hardAlpha" operator="out" />
			<feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.1 0" />
			<feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_433_85" />
			<feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_433_85" result="shape" />
		</filter>
		<filter
			id="filter1_d_433_85"
			x="-41.2075"
			y="23.9625"
			width="2006.13"
			height="1303.07"
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
			<feOffset dy="-10" />
			<feGaussianBlur stdDeviation="10" />
			<feComposite in2="hardAlpha" operator="out" />
			<feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0.275686 0 0 0 0 0.475 0 0 0 1 0" />
			<feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_433_85" />
			<feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_433_85" result="shape" />
		</filter>
	</defs>
</svg>
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
	svg {
		margin-top: 20vh;
		width: 100%;
	}
	.container {
		margin-top: -110vh;
		background-color: $dark-theme;
		@include vert;
		button {
			width: 20%;
			margin: 100px 0;
			height: 9.5vh;
			z-index: 1;
			color: black;
			background-color: $light-blue;
			box-shadow: 0px 4px 40px rgba(0, 0, 0, 0.25);
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
