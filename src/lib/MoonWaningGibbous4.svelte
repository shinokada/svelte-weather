<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'moon waning gibbous 4';
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
    d="M3.74,14.47c0,1.52,0.3,2.98,0.89,4.37s1.39,2.58,2.4,3.59s2.2,1.8,3.59,2.4s2.84,0.89,4.37,0.89
	c2.89-2.39,4.34-6.14,4.34-11.24c0-2.34-0.41-4.47-1.22-6.36s-1.85-3.52-3.11-4.87c-2.03,0-3.91,0.5-5.64,1.51S6.25,7.12,5.24,8.84
	S3.74,12.44,3.74,14.47z"
  />
</svg>

<!--
@component
[Go to docs](https://svelte-weather-icons.codewithshin.com/)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'moon waning gibbous 4';
-->
