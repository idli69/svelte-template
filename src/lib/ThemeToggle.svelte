<script>
    let light = $state(document.documentElement.dataset.theme === "light");

    function toggle() {
        light = !light;
        document.documentElement.dataset.theme = light ? "light" : "dark";
        localStorage.setItem("theme", light ? "light" : "dark");
    }
</script>

<button
    onclick={toggle}
    class="fixed top-5 right-5 rounded-full border border-bd bg-sf px-3 py-1.5 text-fg hover:border-pri transition"
>
    {light ? "☀️" : "🌙"}
</button>
