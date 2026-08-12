<script>
    import Counter from "./lib/Counter.svelte";
    import ThemeToggle from "./lib/ThemeToggle.svelte";
    let name = $state("");
</script>

<main class="min-h-screen bg-bg text-fg flex justify-center">

    <ThemeToggle/>
    <header class="mx-auto max-w-5xl px-5 py-20">
        <p class="font-mono text-sm font-bold text-pri">
            SVELTE 5 + TAILWIND 4 TEMPLATE
        </p>

        <h1 class="mt-6 font-mono font-bold text-[clamp(2rem,6vw,4rem)]">
            Hi, I'm Idli
        </h1>

        <section class="mt-20 p-5 max-w-md border-2 border-pri rounded-lg">
            <label for="name" class="mb-2 text-center block text-mutf">
                Svelte 5 Reactivity
            </label>

            <Counter />

            {#if name}
                <p class="mt-4 text-center text-2xl text-mutf">
                    Hello, <span class="text-fg">{name}</span> 👋
                </p>
            {/if}

            <input
                id="name"
                class="mt-4 w-full rounded-lg border border-bd bg-mut px-4 py-3 text-fg outline-none focus:border-pri"
                type="text"
                placeholder="Input your name..."
                bind:value={name}
            />
        </section>
    </header>
</main>
