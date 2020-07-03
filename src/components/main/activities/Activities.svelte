<script>
  import ActivityItem from "./ActivityItem.svelte";
</script>

<div class="flex flex-row mt-6">
  <div class="flex flex-col flex-shrink w-1/5">
    <h3 class="text-xl font-bold text-black">Daily activity</h3>
    <p class="text-gray text-sm leading-relaxed mt-1">
      Your health plan is also about tapping into resources that can help you
      achieve your health goals.
    </p>
  </div>

  <div class="flex flex-row space-x-10 ml-6 overflow-hidden">
    <ActivityItem title="Steps" icon="feet" value="11 357" update="3m" />
    <ActivityItem
      title="Heart Rate"
      icon="heart"
      value="91"
      unit="bpm"
      update="4h" />
    <!--<ActivityItem title="Sleep" icon="moon" value="7h45m" update="5h" />-->
    <ActivityItem
      title="Weight"
      icon="timer"
      value="56"
      unit="kg"
      update="1d" />
  </div>
</div>
