<script lang="ts">
  export let href: string, text: string;
</script>

<a {href} class="text-white underline-offset-8" class:underline={}>
  {text}
</a>