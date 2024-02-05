<script>
    import logo from "/logos/logo.png";

    //fill in paragraphs from pdf
    const paragraphs = [
        {
            title: "WHO AM I",
            p: ["p1", "p2", "p3"]
        }
    ]

</script>

<main class="font-serif">
    <div class="flex justify-center pt-5 w-4/5 mx-auto">
        <p class="text-6xl text-[#bd243b]">Matrimonies by</p>
        <div class="grid place-content-center ms-3">
            <img class="w-12" src={logo} alt="" />
        </div>
        <p class="text-6xl text-[#bd243b]">ary</p>
        
    </div>
    <!--cool idea: put image wall to scroll over like gune on pc
    and on mobile a carousel of those images (no clue how tf to do it)-->
    <div class="text-center mt-10">
        {#each paragraphs as item}
            <p class="text-3xl">{item.title}</p>
            {#each item.p as p}
                <p>{p}</p>
            {/each}
        {/each}
    </div> 
</main>
