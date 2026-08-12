<script>
    let count = $state(0);
</script>

<section class="mx-auto max-w-sm space-y-4 my-10">
    <p class="text-center text-4xl font-bold">
        {count}
    </p>

    <div class="flex justify-center gap-2">
        <button
            class="rounded bg-slate-800 px-4 py-2 hover:bg-slate-700 transition-transform duration-150 active:scale-95"
            onclick={() => count--}
        >
            −
        </button>

        <button
            class="rounded bg-slate-800 px-4 py-2 hover:bg-slate-700 transition-transform duration-150 active:scale-95"
            onclick={() => count++}
        >
            +
        </button>
    </div>
</section>
