<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'moon waxing gibbous 1';
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
    d="M13.93,14.44c-0.02,4.53,0.33,8.29,1.04,11.27c2.04,0.01,3.93-0.49,5.65-1.49s3.1-2.36,4.11-4.08s1.52-3.61,1.53-5.65
	c0.01-2.04-0.49-3.93-1.49-5.65c-1-1.73-2.36-3.1-4.08-4.11s-3.6-1.52-5.64-1.53C14.32,6.91,13.94,10.66,13.93,14.44z"
  />
</svg>

<!--
@component
[Go to docs](https://svelte-weather-icons.codewithshin.com/)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'moon waxing gibbous 1';
-->
