<script>
    let count = $state(0);
    const increment = () => count++;
    const decrement = () => (count > 0 ? count-- : (count = 0));
</script>

<div class="hero bg-base-300 min-h-screen">
    <div class="hero-content text-center">
        <div class="max-w-md">
            <p class="py-5 text-4xl">
                Count = {count}
            </p>
            <button class="btn btn-accent btn-soft mx-2" onclick={decrement}>
                -
            </button>
            <button class="btn btn-primary btn-soft mx-2" onclick={increment}>
                +
            </button>
        </div>
    </div>
</div>
