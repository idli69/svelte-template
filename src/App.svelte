<script>
    let count = $state(0);
</script>

<main class="flex flex-col items-center justify-center min-h-screen gap-2">
    <h1 class="text-5xl">Hello, World!</h1>

    <span class="mt-5 text-xl text-mist">Count: {count}</span>
    <button class="button" onclick={() => count++}> Increment </button>
</main>

<style></style>
