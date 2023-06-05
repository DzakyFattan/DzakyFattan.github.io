<script>
    export let color = "def";
    export let title = "Title";
    export let description = "Description";
    export let date = "01-01-1970";
</script>

<div class="w-full h-24 grid grid-cols-7">
    <div class="col-span-3 text-end self-center">
        <p class="text-lg font-bold md:text-2xl">{title}</p>
        <p class="text-sm text-neutral-400 md:text-lg">{description}</p>
    </div>
    <div class="flex flex-col justify-self-center w-18">
        <div class="w-1 h-[46px] self-center bg-{color == "start" ? "black" : "rose-600"}"></div>
        <div class="w-4 h-4 bg-rose-600 rounded-full"></div>
        <div class="w-1 h-[46px] self-center bg-{color == "end" ? "black" : "rose-600"}"></div>
    </div>
    <p class="col-span-3 text-lg text-start font-bold self-center md:text-2xl">{date}</p>
</div>