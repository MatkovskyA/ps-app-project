<script setup>

</script>

<template>
	<button class="button font-semibold">
		<slot name="icon"></slot>
		<slot></slot>
		<slot name="minus"></slot>
		<slot name="fla"></slot>
	</button>
</template>

<style scoped>
	.button {
		border: none;
		font-size: 20px;
		border-radius: 10px;
		background: var(--gradient);
		padding: 14px;
		color: var(--color-primary);
		cursor: pointer;
		display: flex;
		gap: 9px;
		align-items: center;
	}

	.button:hover {
		background: var(--gradient-inverted);
	}

</style>
