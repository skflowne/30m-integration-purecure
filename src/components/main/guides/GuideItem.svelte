<script>
  import Progress from "./Progress.svelte";

  export let title = "";
  export let icon;
  export let progress;
  export let gradient;
</script>

<div
  class:bg-grey-100={!gradient}
  style={gradient ? `background: linear-gradient(180deg, white 0%, ${gradient.start} 2.5%, ${gradient.stop} 97.5%, white 100%);` : ''}
  class="p-10 rounded-lg shadow-lg flex flex-col w-full">
  {#if progress}
    <Progress {progress} />
  {/if}
  {#if icon}
    <img class="w-10 ml-auto" src={`/img/${icon}.jpg`} alt="guide-icon" />
  {/if}
  <h5 class="text-xl text-black font-bold">{title}</h5>
</div>
