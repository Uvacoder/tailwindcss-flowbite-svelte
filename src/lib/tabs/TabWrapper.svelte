<script lang="ts">
	import classNames from 'classnames';
	export let divClass: string = 'w-full';
	export let tabStyle: 'default' | 'full' | 'icon' | 'pill' | 'underline' | 'custom' = 'default';
	let tabId: number;
	export let activeTabValue: number;
</script>

<div class={classNames(divClass, $$props.class)}>
	<slot {tabStyle} {tabId} {activeTabValue} />
</div>
