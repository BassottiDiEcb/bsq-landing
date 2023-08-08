<script lang="ts">
  export let href: string, text: string;

  let underline = false;

  function handleClick() {
    const words = window.location.href.split('#')
    console.log(window.location.href, words[1]);
    return words[1] === href
  }
</script>

<a href={`#${href}`} on:click={handleClick} class="text-white underline-offset-8" class:underline={handleClick}>
  {text}
</a>