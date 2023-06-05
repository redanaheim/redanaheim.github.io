<script lang="ts">
	import Tab from "./Tab.svelte";
</script>

<h1 id="projects_title">
	Things I've Created
</h1>

<div id="frontend_projects">
	<a class="card_link" href="https://claritytalentmeasurement.com/roi-2/">
		<div class="card" id="clarity_calculator">
			<h3 class="card_title">
				Return on Investment Calculator: Clarity Talent Measurement
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A calculator which estimates how much Clarity's assessments can save your company. Built with Svelte, TypeScript, and vanilla CSS. Uses the JavaScript autonumeric library for seamless large number inputs. Svelte's efficient reactivity is perfect for a calculator like this.
			</p>
			<img src="./clarity_calculator.png" id="clarity_calculator" alt="ROI Calculator"/>
		</div>
	</a>
	<a href="https://sbbldrugcalculator.github.io" class="card_link">
		<div class="card" id="drugcalculator">
			<h3 class="card_title">
				Drug Sentencing Calculator: Springstead, Bartish, Borgula & Lynch Law, PLLC
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A calculator which gives the user the recommended sentence in months based on the United States Sentencing Commission guidelines for certain drug crimes. <br><Tab/>Users can input any combination of amounts of the hundreds of drugs specified in the Drug Quantity Table, and the calculator handles the conversion to marijuana equivalent weight. <br><Tab/>Factors in all elements of the crime that affect the sentencing range and displays them in a neat table. Also built with Svelte and TypeScript.
			</p>
			<img src="./drug_calculator.png" id="drug_calculator" alt="Drug sentencing calculator"/>
		</div>
	</a>
</div>

<style>
	h1#projects_title {
		text-align: center;
		width: 100%;
	}

	#frontend_projects {
		display: flex;
		width: 93%;
		padding: 20px;
		gap: 2em;
		margin-left: auto;
		margin-right: auto;
	}

	.card, .card_link {
		flex-grow: 1;
		flex-basis: 40%;
		position: relative;
	}

	img {
		width: 100%;
		margin-left: auto;
		margin-right: auto;
		border-radius: 5px;
	}

	.card_link {
		width: 1em;
		z-index: 2;
		display: inline;
		position: relative;
		top: 0.2em;
		left: 0.5em;
	}
</style>
