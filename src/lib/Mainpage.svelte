<script>
    import logo from "/logos/logo.png";
    import img1 from "/images/img1.jpeg";
    import img2 from "/images/img2.jpeg";
    import img3 from "/images/img3.jpeg";


    const paragraphs = [
        {
            title: "<p class=\"text-3xl font-bold text-[#bd243b] text-center\">ABOUT ME</p>",
            p: [
                "<br>"
            ]
        },
        {
            title: "<p class=\"text-3xl\">WHO AM I</p>",
            p: [
                '<p class="pt-2">A qualified celebrant with a passion for creating unforgettable ceremonies<p><br>',
                "<p>A professional singer with 30+ years of experience in Canada and Europe</p>",
                "<ul>",
                    "<li>jazz, pop, soul</li>",
                "</ul><br>",
                "<p>Bilingual English/Italian speaker from Canada</p>",
                "<ul>",
                    "<li>can sing in French and German</li>",
                "</ul><br><br>"
            ],
        },
        {
            title: "<p class=\"text-3xl\">WHY CHOOSE A SINGING CELEBRANT</p>",
            p: [
                '<p class="pt-2">Unforgettable Moments: With a singing celebrant your ceremony will be filled with beautiful melodies and heartfelt performances</p><br>',
                "<p>Personalization: I work closely with you to choose songs that reflect your unique love story</p><br>",
                "<p>Memorable Experience: Your ceremony will move and engage your guests with the enchanting combination of spoken words and live music, leaving a lasting impression.</p><br><br>",
            ],
        },
        {
            title: "<p class=\"text-3xl\">WHY CHOOSE ME AS YOUR SINGING CELEBRANT</p>",
            p: [
                '<p class="pt-2">Warmth and Connection: I strive to create a genuine connection with each couple, making your ceremony a personal and heartfelt experience</p><br>',
                "<p>Professionalism: I bring a high level of professionalism to every ceremony, ensuring a smooth and well-coordinated event</p><br>",
                "<p>Musical Expertise: With years of vocal training and performance experience, I deliver exceptional musical performances tailored to your preferences</p><br><br>",
            ],
        },
        {
            title: "<p class=\"text-3xl font-bold text-[#bd243b] text-center\">SERVICES I OFFER</p>",
            p: [
                "<br>"
            ]
        },
        {
            title: "<p class=\"text-3xl\">1. CERIMONY PLANNING</p>",
            p:[
                "<p class=\"pt-2\">Together, we'll create a personalized ceremony script that reflects your love story</p><br>",
                "<p>I will help you:</p>",
                "<ul>",
                "<li>Choose readings</li>",
                "<li>Choreograph & organize the order of the ceremony entrances, exits, transitions</li>",
                "<li>Incorporate important symbols, stories and metaphors</li>",
                "<li>Honour guests/family members not in attendance</li>",
                "<li>Incorporate symbolic rituals: e.g. handfasting, ring- warming, wooden wine-box time capsule</li>",
                "<li>Select songs and incorporate them seamlessly into the ceremony</li>",
                "</ul><br><br>",
            ]
        },
        {
            title: "<p class=\"text-3xl\">2. LIVE PERFORMANCES</p>",
            p: [
                "<p class=\"pt-2\">I will help you select music that reflects your tastes, style, and mood of the event</p><br>",
                "<p>Musical interludes during key moments such as:</p>",
                "<ul>",
                    "<li>seating guests</li>",
                    "<li>the processional</li>",
                    "<li>recessional</li>",
                    "<li>between poems</li>",
                "</ul><br>",
                "<p>Musical styles include:</p>",
                "<ul>",
                    "<li>Classical</li>",
                    "<li>Pop</li>",
                    "<li>Jazz</li>",
                    "<li>Soul</li>",
                "</ul><br>", 
                "<p>Quality sound will be provided through a professional P.A. system and wireless mic</p><br>"
            ]
        },
        {
            title: "<p class=\"text-3xl\">3. SING ALONG</p>",
            p: [
                "<p class=\"pt-2\">Spread the joy and celebrate with your guests by inviting them to join in singing a favorite song or a chosen group anthem</p>"
            ]
        }
    ];
    
</script>

<main>
    <!-- still have to make everything responsive (it's fucking horrible on mobile atm) -->
    <div class="mx-auto w-2/3 bg-white p-5 my-5 rounded-3xl shadow">
        <div class="flex justify-center w-4/5 mx-auto font-serif">
            <p class="text-6xl text-[#bd243b]">Matrimonies by</p>
            <div class="grid place-content-center ms-3">
                <img class="w-12" src={logo} alt="" />
            </div>
            <p class="text-6xl text-[#bd243b]">ary</p>
        </div>

        <!-- 2 cols bc the images should go on the right -->
        <div class="grid grid-cols-2">
            <div class="text-start text-lg mt-10 pe-5">
                {#each paragraphs as item}
                    {@html item.title}
                    {#each item.p as p}
                        {@html p}
                    {/each}
                {/each}
            </div>
            <div class="ps-5 mt-10 grid grid-cols-1 gap-5 place-content-between">
                <img class="rounded-3xl" src="{img1}" alt="">
                <img class="rounded-3xl" src="{img2}" alt="">
                <img class="rounded-3xl" src="{img3}" alt="">
            </div>
        </div>
    </div>
</main>
