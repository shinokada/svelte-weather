<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'moon waning gibbous 5';
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
    d="M3.74,14.47c0,2.03,0.5,3.91,1.51,5.63s2.37,3.09,4.09,4.09s3.6,1.51,5.63,1.51c2.17-2.75,3.25-6.5,3.25-11.24
	c0-3.96-1.08-7.71-3.25-11.24c-2.03,0-3.91,0.5-5.63,1.5S6.26,7.1,5.25,8.83S3.74,12.44,3.74,14.47z"
  />
</svg>

<!--
@component
[Go to docs](https://svelte-weather-icons.codewithshin.com/)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'moon waning gibbous 5';
-->
