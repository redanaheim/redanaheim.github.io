<script lang="ts">
	import Tab from "./Tab.svelte";	
</script>

<h1 id="projects_title">
	Things I've Created: Front-end
</h1>
<div id="frontend_projects" class="projects_container">
	<a class="card_wrap_link" href="https://claritytalentmeasurement.com/roi-2/">
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
	<a href="https://sbbldrugcalculator.github.io" class="card_wrap_link">
		<div class="card" id="drugcalculator">
			<h3 class="card_title">
				Drug Sentencing Calculator: Springstead, Bartish, Borgula & Lynch Law, PLLC
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A calculator which gives the user the recommended sentence in months based on the United States Sentencing Commission guidelines for certain drug crimes. <br><Tab/>Users can input any combination of amounts of the hundreds of drugs specified in the Drug Quantity Table, and the calculator handles the conversion to marijuana equivalent weight. Then, based on the quantity of marijuana equivalent weight, it outputs a base "offense level." <br><Tab/>Factors in all elements of the crime that affect the sentencing range and displays them in a neat table. Also built with Svelte and TypeScript.
			</p>
			<img src="./drug_calculator.png" id="drug_calculator" alt="Drug sentencing calculator"/>
		</div>
	</a>
</div>
<h1 id="projects_title_backend">
	Back-end
</h1>
<div class="projects_container" id="backend_projects">
	<a class="card_wrap_link" href="https://github.com/redanaheim/electron-tas-ui">
		<div class="card" id="electron_tas_ui">
			<h3 class="card_title">
				Electron TAS UI
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A specialized application built for writing scripts for [T]ool-[A]ssisted [S]peedruns on the Nintendo Switch, a game console. Essentially, it allows the user to draw out what buttons they want to be pressed on what frames of gameplay, and the program will press them for you. It also bundles a built-in scripting language compiler and can export files to the Switch for you via FTP.<br><Tab/>This application is now obsolete and not maintained due to advancements in Switch emulation technology. It was written in Electron using vanilla TypeScript without a framework.
			</p>
			<img src="./electron_tas_ui.png" id="electron_tas_ui" alt="Electron TAS UI windows"/>
		</div>
	</a>

</div>
<style>
	h1, h2, h3, h4, h5 {
		text-align: center;
		width: 100%;
	}

	.projects_container {
		flex-direction: row;
		display: flex;
		width: 93%;
		padding: 20px;
		gap: 2em;
		margin-left: auto;
		margin-right: auto;
		flex-wrap: wrap;
		justify-content: space-evenly;
		align-items: stretch;
	}

	.card, .card_wrap_link {
		flex-grow: 1;
		flex-basis: 570px;
		position: relative;
		min-width: 570px;
		width: 85%;
		margin-left: auto;
		margin-right: auto;
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
