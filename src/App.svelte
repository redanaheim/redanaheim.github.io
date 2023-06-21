<script lang="ts">
    import { onMount } from "svelte";
    import Projects from "./Projects.svelte";
    import ThemeToggle from "./ThemeToggle.svelte";

    const change_theme = () => {
	document.documentElement.classList.toggle("dark")
	document.body.classList.toggle("dark")
    }

    let header: HTMLHeadingElement;

    onMount(() => {
	    header.addEventListener("click", change_theme)
    })

</script>


<h1 bind:this={header}>
	Gary Springstead • Software Development & Web Design
</h1>

<div class="info">
	<div class="github_profile socials card">
		<a href="https://github.com/redanaheim/">	
			<img id="github_logo" src="github_logo.png" alt="GitHub logo"/>redanaheim
		</a>
	</div>
	<div class="gmail socials card">
		<a href="mailto:garyspringstead1107@gmail.com">
			<img id="gmail_logo" src="gmail_logo.png" alt="G-Mail logo"/>garyspringstead1107@gmail.com
		</a>
	</div>
	<div class="uofm socials card">
		<a href="mailto:elevengs@umich.edu">
			<img id="uofm_logo" src="uofm_logo.png" alt="University of Michigan Block M"/>elevengs@umich.edu
		</a>
	</div>
	<div class="linkedin socials card">
		<a href="https://www.linkedin.com/in/gary-springstead-73a183277/">
			<img id="linkedin_logo" src="linked_in.png" alt="LinkedIn logo"/>Gary Springstead
		</a>
	</div>
</div>
<Projects></Projects>
 
<style>
	#toggle {
		margin-right: 5px;
		margin-left: 95%;
		display: inline;
	}

	h1 {
		text-align: center;
		width: 100%;
	}

	.info {
		margin-left: auto;
		margin-right: auto;
		justify-content: center;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		column-gap: 1em;
		max-width: 800px;
		width: 80%;
	}

	div.socials {
		vertical-align: bottom;
		text-align: center;
		width: max-content;
		margin-top: 0.5em;
		margin-bottom: 0.5em;
	}

	.socials > a {
		display: block;
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
