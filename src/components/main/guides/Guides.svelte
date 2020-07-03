<script>
  import GuideItem from "./GuideItem.svelte";
</script>

<div>
  <h2 class="text-xl">Health Guides</h2>
  <div class="flex flex-row overflow-hidden space-x-10">
    <GuideItem
      title="Diet & Excercise"
      gradient={{ start: '#e6dfff', stop: '#d5ecfe' }} />
    <GuideItem
      title="Screening & Tests"
      icon="stetoscope"
      progress={{ current: 9, max: 15, label: 'Check your health list ' }} />
    <GuideItem title="Rest & Relaxation" />
  </div>
</div>
