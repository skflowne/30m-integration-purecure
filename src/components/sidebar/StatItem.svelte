<script>
  export let label = "";
  export let value = "";
  export let unit = "";
</script>

<div class="flex flex-col p-2">
  <span class="text-blue uppercase">{label}</span>
  <div>
    <span class="text-black text-xl font-bold">{value}</span>
    <span class="">{unit}</span>
  </div>

</div>
