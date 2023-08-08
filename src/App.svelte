<script lang="ts">
  import Button from "./components/Button.svelte"
import NavigationLink from "./components/NavigationLink.svelte";
</script>

<div class="font-montserrat">
    <section class="h-screen bg-blue-300">
        <header class="flex justify-around p-8">
          <h1 class="font-bold text-2xl text-white">
              BSQ
          </h1>
          <nav class="flex gap-x-4">
            <NavigationLink href="home" text="Home" />
            <NavigationLink href="about_us" text="About us" />
          </nav>
        </header>
        <div class="h-[calc(100%-96px)] flex justify-center items-center text-white">
            <div class="flex flex-col gap-y-8 items-center justify-center">
                <p class="text-7xl font-bold">BSQ</p>
                <hr class="border border-b-white w-full" />
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, commodi.</p>
                <Button text="Scopri di più" />
            </div>
        </div>
    </section>
</div>
