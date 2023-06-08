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
				Electron TAS UI: Independent
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A specialized application built for writing scripts for [T]ool-[A]ssisted [S]peedruns on the Nintendo Switch game console. Essentially, it allows the user to draw out what buttons they want to be pressed on what frames of gameplay, and the program will press them for you. It also bundles a built-in scripting language compiler and can export files to the Switch for you via FTP.<br><Tab/>This application is now obsolete and not maintained due to advancements in Switch emulation technology. It was written in Electron using vanilla TypeScript without a framework.
			</p>
			<img src="./electron_tas_ui.png" id="electron_tas_ui" alt="Electron TAS UI windows"/>
		</div>
	</a>
	<a class="card_wrap_link" href="https://github.com/redanaheim/typedyno">
		<div class="card" id="typedyno">
			<h3 class="card_title">
				TypeDyno: Independent
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A custom-built Node.js Discord bot written in TypeScript that uses PostgreSQL for its databases. It ships with a module system for easy additions and automatically configures both text-based and slash-based commands. <br><Tab/>Internal command APIs make it easy to define the syntax for a command declaratively, and arguments users give can be checked by the built in runtime type checking system, giving clear error messages easily. TypeScript's flexible type system enables all argument types (including users, specified by ID or @, or custom enums) to be shown while writing command handlers.
			</p>
			<img src="./typedyno_usage.png" id="typedyno_usage" alt="TypeDyno usage"/>
		</div>
	</a>
</div>
<h1 id="projects_title_misc">
	Miscellaneous
</h1>
<div class="projects_container" id="misc_projects">
	<a class="card_wrap_link" href="https://github.com/redanaheim/scratchthat/">
		<div class="card" id="scratchthat">
			<h3 class="card_title">
				Scratch That: Independent
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A Firefox extension which allows you to substitute arbitrary text on all pages, including dynamically loaded content.
				It was intended to be used primarily for privacy on social media, but has a wide variety of other use cases.<br><Tab/>Specifiers can be very simple or very complex using regular expressions. Replacement text may include captured text from the original, random replacements from a list of possible strings, or just plaintext.
			</p>
			<img src="./scratch_that.png" id="scratch_that" alt="Scratch That usage"/>
		</div>
	</a>
	<a href="https://gist.github.com/redanaheim/b89e7cf3726633319b6d3bfa8141cf17" class="card_wrap_link">
		<div class="card" id="parametric_shader">
			<h3 class="card_title">
				Metal Parametric Curve Shader: Independent
				<img src="./link.png" class="card_link" alt="Link"/>
			</h3>
			<p class="card_subtitle">
				<Tab/>A GPU shader written in Metal which renders an arbitrary parametric curve in 2D space. The motivation for this was for an ML project in which the model would be taught a mapping to a bezier curve, but I found an easier way to accomplish the goal that did not require a bezier curve.
				<Tab/>The shader is efficient (it can run at over 100 fps on my laptop with very high samples) and correct, meaning it does not approximate the curve by lines or make other quality compromises. It accomplishes this by calculating the winding number of the curve for each pixel. I wrote a futher optimized version which takes advantage of reused calculations in PyTorch.
			</p>
			<div class="img_wrapper">
				<img src="./parametric_shader.png" alt="Parametric Shader producing a heart" id="parametric_shader">
			</div>
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

	.img_wrapper {
		text-align: center;
		width: 100%;
	}

	#parametric_shader {
		width: 75%;
	}
</style>
