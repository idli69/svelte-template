<script>
    import Counter from "./lib/Counter.svelte";
</script>

<main class="min-h-screen bg-slate-950 text-slate-100">
    <header class="mx-auto max-w-8xl px-6 py-12 sm:px-10 lg:px-16">
        <h1
            class="max-w-5xl font-mono text-[clamp(3rem,8vw,8rem)] font-bold leading-[0.9] tracking-tight"
        >
            Hi, I'm Idli.
        </h1>

        <p
            class="mt-8 max-w-2xl text-[clamp(1.1rem,2vw,1.5rem)] leading-relaxed text-slate-400"
        >
            A lightweight Svelte + Tailwind starter template for my projects.
        </p>
    </header>

    <section class="mx-auto max-w-7xl px-6 pb-16 sm:px-10 lg:px-16">
        <Counter />
    </section>
</main>
