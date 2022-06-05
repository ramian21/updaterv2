<script lang="ts">
	import Actions from "@smui/card/src/Actions.svelte";
	import Card from "@smui/card/src/Card.svelte";
	import Media from "@smui/card/src/Media.svelte";
	import { each } from "svelte/internal";
	import SetThumbnail from "./lib/components/SetThumbnail.svelte";

	let thumbnailData = [
		{
			roundTitle: "winners pools",
			player1Tag: "player 1",
			player2Tag: "player 2",
		},
		{
			roundTitle: "winners pools",
			player1Tag: "player 3",
			player2Tag: "player 4",
		},
		{
			roundTitle: "winners pools",
			player1Tag: "player 5",
			player2Tag: "player 6",
		},
	];
</script>

<main>
	{#each thumbnailData as datapoint}
		<SetThumbnail {...datapoint} />
	{/each}
</main>

<svelte:head>
	<link
		rel="stylesheet"
		href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,600,700"
	/>
</svelte:head>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
