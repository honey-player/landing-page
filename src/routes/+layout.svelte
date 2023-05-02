<script>
	import { onMount } from 'svelte';

	import Header from './Header.svelte';

	import './styles.css';

	let clientOS = '';
	onMount(() => {
		const os = navigator.userAgent;

		let finalOs = '';

		if (os.search('Windows') !== -1) {
			finalOs = 'win';
		} else if (os.search('Mac') !== -1) {
			finalOs = 'mac';
		} else if (os.search('X11') !== -1 && !(os.search('Linux') !== -1)) {
			finalOs = 'linux';
		} else if (os.search('Linux') !== -1 && os.search('X11') !== -1) {
			finalOs = 'linux';
		}

		clientOS = finalOs;
	});
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<a href={`https://download.honeyplayer.com?os=${clientOS}`}
			><button class="download">Download Now</button></a
		>
		<span>
			or, visit <a href="https://download.honeyplayer.com">download.honeyplayer.com</a> to download the
			latest release for any platform
		</span>
		<p>
			Play videos directly through the internet/torrent and create room to watch together, <strong
				>absolutely free!</strong
			>
		</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		width: 100%;
		max-width: 64rem;
		padding: 1em 1em 0em 1em;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.download {
		display: inline-block;
		background: #111;
		color: #eee;
		font-weight: 500;
		padding: 1rem 1.5rem;
		margin: 1rem 0 0 0;
		text-decoration: none;
		border-radius: 2rem;
	}
	.download:hover {
		background: var(--color-theme-1);
		color: white;
		outline: none;
		cursor: pointer;
	}

	span {
		font-size: 0.8rem;
		margin: 1rem 0 0 0;
		color: #777;
		text-align: center;
	}

	p {
		font-size: 0.8rem;
		text-align: center;
	}

	a {
		font-weight: bold;
	}
</style>
