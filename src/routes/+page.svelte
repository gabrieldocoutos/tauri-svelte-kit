<script lang="ts">
	let content = "";

	function handleKeyPress(event: KeyboardEvent) {
		content += event?.key;
	}
</script>

<div>
	<div on:keydown={handleKeyPress} tabindex="-1" class="container">
		{content}
	</div>
</div>

<style>
	.container {
		width: 200px;
		height: 200px;
		background-color: red;
	}
</style>
