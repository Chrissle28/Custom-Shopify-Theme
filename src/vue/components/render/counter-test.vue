<template>
	<div class="flex items-center gap-4">
		<button
			class="p-1 text-white bg-black rounded-full"
			@click="counter -= 1"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="-5 -11 24 24"
				width="24"
				fill="currentColor"
			>
				<path d="M1 0h12a1 1 0 0 1 0 2H1a1 1 0 1 1 0-2z"></path>
			</svg>
		</button>
		<span>Counter: {{ counter }}</span>
		<button
			class="p-1 text-white bg-black rounded-full"
			@click="counter += 1"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="-4.5 -4.5 24 24"
				width="24"
				fill="currentColor"
			>
				<path
					d="M8.9 6.9v-5a1 1 0 1 0-2 0v5h-5a1 1 0 1 0 0 2h5v5a1 1 0 1 0 2 0v-5h5a1 1 0 1 0 0-2h-5z"
				></path>
			</svg>
		</button>
	</div>
</template>

<script setup>
import { ref } from 'vue';

const counter = ref(0);
</script>
