<script>
  export let progress = { current: 0, max: 1, label: "" };
  $: percentage = (progress.current / progress.max) * 100;
</script>

<div class="progress">
  <div>
    <span class="font-bold">{progress.current}&nbsp;/</span>
    <span>&nbsp;{progress.max}</span>
    <div class="bar bg-gray">
      <div class="filler bg-blue" style={`width:${percentage}%`} />
    </div>
    <p class="text-gray">{progress.label}</p>
  </div>
</div>
