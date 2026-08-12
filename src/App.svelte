<script>
    import Counter from "./lib/Counter.svelte";

    let name = $state("");
</script>

<main class="min-h-screen bg-slate-950 text-slate-100 flex">
    <header class="mx-auto max-w-5xl px-5 py-25 sm:px-10 lg:px-15">
        <div class="max-w-4xl">
            <p class="font-mono text-sm font-bold text-orange-500">
                SVELTE 5 + <span class="text-blue-400">TAILWIND 4</span>
            </p>

            <h1 class="mt-6 font-mono text-4xl font-bold tracking-tight">
                Hi, I'm Idli.
            </h1>

            <p class="mt-8 max-w-2xl text-xl leading-relaxed text-slate-400">
                A minimal starter template for my projects.
            </p>
        </div>

        <section class="mt-16 max-w-md">
            <label for="name" class="mb-2 block text-md text-slate-400">
                Svelte 5 Reactivity
            </label>

            <Counter />

            {#if name}
                <p class="text-slate-400 text-center text-3xl my-4">
                    Hello, <span class="text-slate-100">{name}</span> 👋
                </p>
            {/if}
            <input
                id="name"
                class="w-full rounded-lg border border-slate-800 bg-slate-800 px-4 py-3 outline-none transition focus:border-orange-500"
                type="text"
                placeholder="Input your name..."
                bind:value={name}
            />
        </section>
    </header>
</main>
