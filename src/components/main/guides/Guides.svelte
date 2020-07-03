<script>
  import GuideItem from "./GuideItem.svelte";
</script>

<div>
  <h2 class="text-2xl font-bold">Health Guides</h2>
  <div class="flex flex-row overflow-hidden space-x-10 py-4 mb-4">
    <GuideItem
      title="Diet & Excercise"
      gradient={{ start: '#e6dfff', stop: '#d5ecfe' }} />
    <GuideItem
      title="Screening & Tests"
      icon="stetoscope"
      progress={{ current: 9, max: 15, label: 'Check your health list ' }} />
    <GuideItem
      title="Rest & Relaxation"
      gradient={{ start: '#efffb6', stop: '#c1fdd4' }} />
  </div>
</div>
