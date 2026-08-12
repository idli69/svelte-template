<script>
    let count = $state(0);
</script>

<section class="mx-auto max-w-sm space-y-2 p-5 my-10 border-2 border-mut rounded-lg">
    <p class="text-center text-4xl font-bold text-fg">
        {count}
    </p>
    <div class="flex justify-center gap-2">
        <button
            class="rounded bg-mut px-4 py-2 text-fg hover:bg-pri hover:text-prif transition-transform duration-150 active:scale-95"
            onclick={() => count--}
        >
            −
        </button>
        <button
            class="rounded bg-mut px-4 py-2 text-fg hover:bg-pri hover:text-prif transition-transform duration-150 active:scale-95"
            onclick={() => count++}
        >
            +
        </button>
    </div>
</section>
