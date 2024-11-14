<script lang="ts">
	import type { DeviceType } from '../types';

	let props: DeviceType = $props();
</script>

<div class="flex">
	<label>
		<button class="">{props.name}</button>
	</label>
</div>
