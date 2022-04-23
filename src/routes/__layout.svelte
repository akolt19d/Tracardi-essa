<nav>
	<img src={`./logo.svg`} alt="Tracardi logo" />
	<h3 class="blue">TRACARDI</h3>
	<ul>
		<a href="/">
			<li>Home</li>
		</a>
		<a href="/customers">
			<li>Customers</li>
		</a>
		<li>Contact</li>
		<li>Docs</li>
		<a href="/pricing">
			<li>Pricing</li>
		</a>
	</ul>
</nav>
<slot />

<style lang="scss">
	nav {
		width: 100%;
		min-height: 6rem;
		@include fc;
		background: darken($bg-l, 1);
		margin: 0;
		transition: $theme-fade;
		position: fixed;
		top: 0;
		left: 0;
		z-index: 1000;
		h3 {
			margin: 0 2rem 0 0.3rem;
		}
		ul {
			display: flex;
			justify-content: space-evenly;
			list-style: none;
			a {
				text-decoration: none;
				color: black;
			}
			li {
				margin: 20px;
				font-weight: bold;
				font-size: 80%;
				transition: 0.2s;
				cursor: pointer;
			}
			li:hover {
				color: $blue;
			}
		}
	}
	@media screen and (max-width: 600px) {
		nav {
			display: none;
		}
	}
</style>
