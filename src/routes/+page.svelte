<script>
	import honey_player_torrent from '$lib/images/honey-player-torrent.png';
</script>

<svelte:head>
	<title>Honey Player - The modern media player for friends</title>
	<meta name="description" content="Download now and stream videos through the internet" />
</svelte:head>

<section>
	<span class="welcome">
		<img src={honey_player_torrent} alt="Honey Player" />
	</span>

	<h1>Honey Player</h1>
	<h2>
		The&nbsp;<strong>modern</strong>
		media player for friends
	</h2>
	<h3>Stream videos instantly ⟡ Create room & watch together ⟡ Multi-stream support</h3>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	.welcome {
		display: block;
		position: relative;
		width: 85%;
		height: 0;
		padding: 0 0 46% 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
		margin: 1rem 0 0 0;
		border-radius: 10px;
		box-shadow: 10px 10px 15px rgba(76, 79, 91, 0.5), -10px -10px 15px rgba(65, 69, 88, 0.12);
	}

	h1 {
		width: 100%;
		font-size: 4rem;
		font-weight: normal;
		letter-spacing: 0.1rem;
		margin: 2rem 0 0 0;
		text-align: center;
	}

	h2 {
		font-size: 1.6rem;
		margin: 1rem 0 0 0;
		text-align: center;
	}

	h3 {
		font-weight: 100;
		text-align: center;
		margin: 1.3rem 0 0 0;
	}
</style>
