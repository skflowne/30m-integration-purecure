<script>
  import StatItem from "./StatItem.svelte";
</script>

<style>
  .stats {
    border-radius: 20px;
  }
</style>

<div class="stats shadow-xl flex flex-col p-4 pb-6">
  <StatItem label="Age" value="23" unit="yo" />
  <StatItem label="Weight" value="55" unit="kg" />
  <StatItem label="Height" value="167" unit="cm" />
</div>
