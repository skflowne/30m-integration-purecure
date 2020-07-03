<script>
  export let icon;
  export let name;
  export let active = false;
</script>

<div
  class="flex flex-row items-center py-2"
  class:text-gray={!active}
  class:text-black={active}>
  <img class="mr-4" src={`/img/${icon}.jpg`} alt={icon} />
  <a class="text-left" href="#">{name}</a>
</div>
