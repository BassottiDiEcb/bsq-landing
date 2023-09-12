<script lang="ts">
  export let title: string;
</script>

<div class="p-4 border rounded-lg shadow col-span-12 md:col-span-6">
  <div class="border-b-2 border-slate-900 font-bold uppercase mb-4">{title}</div>

  <p>
    <slot />
  </p>
</div>