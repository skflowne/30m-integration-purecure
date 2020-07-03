<script>
  export let value;
  export let unit;
  export let title;
  export let update;
  export let icon;
</script>

<div class="flex flex-col rounded-lg border-bluegray border p-6 w-48">
  <div class="flex flex-grow">
    <h6 class="inline text-sm font-bold uppercase">{title}</h6>
    <img
      class="relative top-10 inline self-end"
      src={`/img/${icon}.jpg`}
      alt="activity-icon" />
  </div>

  <div class="flex flex-col">
    <div>
      <span class="text-xl font-bold">{value}</span>
      {#if unit}
        <span>{unit}</span>
      {/if}
    </div>
    <p class="text-gray text-sm">Last update: {update}</p>
  </div>
</div>
