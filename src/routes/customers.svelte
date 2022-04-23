<script>
	import Content from '../components/CustomersSection/content.svelte';
	import Retail from '../components/CustomersSection/retail.svelte';
	import FinancialServices from '../components/CustomersSection/FinancialServices.svelte';
</script>

<Content />
<Retail />
<FinancialServices />

<style lang="scss">
	:global(*) {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}
	:global(body) {
		overflow-x: hidden;
		min-height: 200vh;
		color: #111;
		background-color: #f5f5f5;
		transition: $theme-fade;
		overflow-x: hidden;
		font-family: $font;
	}
</style>
