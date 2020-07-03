<script>
  import Progress from "./Progress.svelte";

  export let title = "";
  export let icon;
  export let progress;
  export let gradient;
</script>

<style>
  .guide {
    height: 320px;
  }
</style>

<div
  class:bg-grey-100={!gradient}
  style={gradient ? `background: linear-gradient(180deg, ${gradient.start} 25%, ${gradient.stop} 75%);` : ''}
  class="p-10 rounded-lg shadow-lg flex flex-col guide">
  <div class="flex flex-grow flex-col">
    {#if progress}
      <Progress {progress} />
    {/if}
  </div>

  {#if icon}
    <img
      class="mr-0 w-10 ml-auto self-end"
      src={`/img/${icon}.jpg`}
      alt="guide-icon" />
  {/if}
  <h5 class="text-xl text-black font-bold self-end text-right">{title}</h5>
</div>
