<script>
    export let title;
    export let description;
    export let date;
</script>

<div class="w-full h-24 grid grid-cols-5 items-center">
    <div class="col-span-2 text-end">
        <p class="text-2xl font-bold">{title}</p>
        <p class="text-lg text-slate-400">{description}</p>
    </div>
    <div class="justify-self-center">
        <div class="w-8 h-8 bg-rose-600 rounded-full"></div>
    </div>
    <p class="col-span-2 text-2xl text-start font-bold">{date}</p>
</div>