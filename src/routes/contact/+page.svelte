<svelte:head>
	<title>Contact || Honey Player - The modern media player for friends</title>
	<meta name="description" content="Contact Honey Player" />
</svelte:head>

<div class="text-column">
	<h1>Contact Us</h1>

	<p>
		Do you have some query about how we roll? Or you found a horrible bug and want us to know? Maybe
		you see potential in Honey Player and want to be Elon Musk and make us twitter? Reach out to us
		at:
	</p>
	<center><a href="mailto:sunim.honeyplayer@gmail.com">sunim.honeyplayer@gmail.com</a></center>

	<div class="example">
		<span class="close">l</span>
		<span class="missing">e</span>
		<span class="close">t</span>
		<span class="missing">`</span>
		<span class="close">s</span>
		<span class="exact">p</span>
		<span class="exact">a</span>
		<span class="exact">r</span>
		<span class="exact">t</span>
		<span class="exact">y</span>
	</div>
</div>

<style>
	span {
		display: inline-flex;
		justify-content: center;
		align-items: center;
		font-size: 0.8em;
		width: 2.4em;
		height: 2.4em;
		background-color: white;
		box-sizing: border-box;
		border-radius: 2px;
		border-width: 2px;
		color: #000000b3;
	}

	.missing {
		background: rgba(255, 255, 255, 0.5);
		color: #00000080;
	}

	.close {
		border-style: solid;
		border-color: var(--color-theme-2);
	}

	.exact {
		background: var(--color-theme-2);
		color: white;
	}

	.example {
		display: flex;
		justify-content: center;
		margin: 2rem 0;
		gap: 0.2rem;
	}

	.example span {
		font-size: 1.4rem;
	}

	p span {
		position: relative;
		border-width: 1px;
		border-radius: 1px;
		font-size: 0.4em;
		transform: scale(2) translate(0, -10%);
		margin: 0 1em;
	}
</style>
