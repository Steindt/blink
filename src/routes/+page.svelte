<script lang="ts">
	import Device from '$lib/device.svelte';
	import type { DeviceType } from '../types';

	let mockData: DeviceType[] = [
		{ name: 'Device 1', ip: '127.0.0.1' },
		{ name: 'Device 2', ip: '127.0.0.1' }
	];

	let props = mockData;
</script>

<main class="h-screen w-screen">
	<h1>Home page</h1>
	{props.map((value: DeviceType, index: number, array: DeviceType[]) => {
		<Device props={value} />;
	})}
</main>
