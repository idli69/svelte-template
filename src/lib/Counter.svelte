<script>
    let count = $state(0);
</script>

<section
    class="mx-auto max-w-xl rounded-2xl border border-slate-800 bg-slate-900 p-6 shadow-xl"
>
    <div class="mb-8">
        <p class="font-mono text-md text-center text-orange-400">
            REACTIVE COMPONENT EXAMPLE
        </p>
    </div>

    <output
        class="block rounded-lg bg-slate-950 px-6 py-8 text-center font-mono text-4xl font-bold"
    >
        {count}
    </output>

    <div class="mt-4 grid grid-cols-2 gap-3">
        <button
            class="rounded-lg bg-slate-800 px-4 py-3 font-medium transition hover:bg-slate-700 active:scale-[0.98]"
            onclick={() => count++}
        >
            Increase
        </button>

        <button
            class="rounded-lg bg-slate-800 px-4 py-3 font-medium transition hover:bg-slate-700 active:scale-[0.98]"
            onclick={() => count--}
        >
            Decrease
        </button>
    </div>
</section>
