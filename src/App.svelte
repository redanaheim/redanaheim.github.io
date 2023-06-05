<script lang="ts">
    import Projects from "./Projects.svelte";
</script>

<h1>
	Gary Springstead - Software Development & Web Design
</h1>

<table class="info">
	<tr class="socials">
		<td class="github_profile socials card">
			<a href="https://github.com/redanaheim/">	
				<img id="github_logo" src="github_logo.png" alt="GitHub logo"/>redanaheim
			</a>
		</td>
		<td class="gmail socials card">
			<a href="mailto:garyspringstead1107@gmail.com">
				<img id="gmail_logo" src="gmail_logo.png" alt="G-Mail logo"/>garyspringstead1107@gmail.com
			</a>
		</td>
		<td class="uofm socials card">
			<a href="mailto:elevengs@umich.edu">
				<img id="uofm_logo" src="uofm_logo.png" alt="University of Michigan Block M"/>elevengs@umich.edu
			</a>
		</td>
	</tr>
</table>
<Projects></Projects>

<style>
	h1 {
		text-align: center;
		width: 100%;
	}

	.info {
		display: table;
		margin-left: auto;
		margin-right: auto;
		justify-content: center;
		display: flex;
	}

	td.socials {
		vertical-align: bottom;
		width: 20em;
		text-align: center;
		margin-left: 1em;
		margin-right: 1em;
		display: inline-block;
		width: max-content;
	}

	.socials > a > img {
		margin-right: 1em;
		vertical-align: bottom;
		height: 1.5em;
		box-sizing: content-box;
	}

	#github_logo {
		filter: var(--invert-filter);
	}

</style>
