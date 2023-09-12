<script lang="ts">
  export let title: string;
</script>

<h1 class="font-bold text-2xl">{title}</h1>

<div class="grid grid-cols-12 gap-4">
  <slot />
</div>