<script>
	import honey_player_start from '$lib/images/honey-player-start.png';
	import honey_player_url from '$lib/images/honey-player-url.png';
	import honey_player_only from '$lib/images/honey-player-only.png';
</script>

<svelte:head>
	<title>About || Honey Player - The modern media player for friends</title>
	<meta name="description" content="About Honey Player" />
</svelte:head>

<div class="text-column">
	<h1>About Honey Player</h1>

	<p>
		Introducing the most feature-packed video player ever made, but not made for offline media
		(yet).
	</p>

	<p>
		It adopts the modern design language, taking inspiration from IINA and Soda Player, while still
		under development to make it feature rich. It does come with a lot of batteries, like a lot.
	</p>

	<div>
		<p>Batteries:</p>
		<ul>
			<li>Picture in Picture</li>
			<li>Direct online streams</li>
			<li>Play Torrent videos instantly</li>
			<li>Support multi-media within the magnet link</li>
			<li>Play subtitles in sync</li>
			<li>Only host downloads the videos and others stream (under LAN)</li>
			<li>Directly create and share room id, no hassle</li>
		</ul>
	</div>

	<div>
		<br />
		<img src={honey_player_start} alt="Honey Player Start" width="250" height="auto" />
		<img src={honey_player_url} alt="Honey Player Url" width="250" height="auto" />
		<img src={honey_player_only} alt="Honey Player Only" width="250" height="auto" />
	</div>
</div>

<style>
	img {
		margin: 0.1em;
		border-radius: 5px;
		box-shadow: 5px 5px 8px rgba(76, 79, 91, 0.5), -5px -5px 8px rgba(65, 69, 88, 0.12);
	}
</style>
