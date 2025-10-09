<script setup>

</script>

<template>
	<button class="button">
		<slot></slot>
	</button>
</template>

<style scoped>
	.button {
		width: 335px;
		font-family: var(--font-secondary);
		border: none;
		border-radius: 100px;
		font-size: 24px;
		line-height: 36px;
		background: var(--color-bg-button2);
		padding: 16px 10px;
		color: var(--color-primary);
		cursor: pointer;
	}
</style>
