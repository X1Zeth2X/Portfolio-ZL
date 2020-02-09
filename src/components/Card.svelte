<script>
  export let title;
  export let color = 'bg-white';
  export let hover = false;
  export let width;
</script>

<style>
  .elevate {
    transition: 0.2s ease-in-out;
  }
  .elevate:hover,

  .elevate:active{
    transform: translateY(5px) !important;
  }
</style>

<div class="{color} {width} {hover ? 'hover:shadow-md elevate' : ''} rounded-lg shadow-2xl">
  <slot name="image"/>

  <div class="p-5">
    <h1 class="font-extrabold text-3xl">{ title }</h1>

    <slot />
  </div>
</div>