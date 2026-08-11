<script>
    import Counter from "./lib/Counter.svelte";
</script>

<main class="bg-slate-800 text-slate-100 min-h-screen">
    <header class="flex flex-col p-5">
        <h1 class="text-[clamp(2rem,5vw,6rem)] font-mono">Hi, I'm Idli</h1>
        <h2 class="self-end text-[clamp(1.2rem,2vw,3rem)]">
            This is a <span class="text-orange-700"><u>SvelteJS</u></span> Template
            made for my projects.
        </h2>
    </header>
    <section class="flex justify-center p-10">
        <Counter />
    </section>
</main>
