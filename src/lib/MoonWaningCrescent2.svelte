<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'moon waning crescent 2';
</script>

<svg
  version="1.1"
  id="Layer_1"
  xmlns="http://www.w3.org/2000/svg"
  xmlns:xlink="http://www.w3.org/1999/xlink"
  x="0px"
  y="0px"
  width={size}
  height={size}
  {...$$restProps}
  {role}
  aria-label={ariaLabel}
  fill={color}
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
  viewBox="0 0 30 30"
  style="enable-background:new 0 0 30 30;"
  xml:space="preserve"
>
  <path
    d="M3.74,14.44c0,2.04,0.5,3.93,1.51,5.65s2.37,3.1,4.1,4.1s3.61,1.51,5.65,1.51c-2.01-2.74-3.02-6.5-3.02-11.26
	c0-3.98,1.01-7.73,3.02-11.25c-2.04,0-3.93,0.5-5.65,1.51s-3.1,2.37-4.1,4.09S3.74,12.4,3.74,14.44z"
  />
</svg>

<!--
@component
[Go to docs](https://svelte-weather-icons.codewithshin.com/)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'moon waning crescent 2';
-->
