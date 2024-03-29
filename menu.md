# Menu Page
## **Note: KEEP EXTERNAL CSS FILE AND IMAGES AT PROPER HIERARCHY**.
    <!doctype html>
    <html class="dark">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link href="dist/output.css" rel="stylesheet">
        <script type="module" src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.esm.js"></script>
        <script src="https://cdn.lordicon.com/fudrjiwc.js"></script>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Domine:wght@500&family=Jost:wght@500&family=Warnes&display=swap" rel="stylesheet">

    </head>

    <body class="font-domine">

        <header
            class=" sticky top-0 z-20
                bg-purple-100 text-purple-800  
                    w-full h-12 md:h-auto 
                dark:text-purple-100 dark:bg-slate-800 shadow-md dark:shadow-zinc-700">
            <div class="    flex flex-row justify-between md:items-end
                            px-5 md:px-10 py-2">
                <div class="md:hidden" onclick="toggleMenu('open')">
                    <ion-icon size="large" name="menu-outline"></ion-icon>
                </div>
                <div class="relative">
                    <a href="index.html">
                        <div
                            class=" absolute top-0 z-10
                                    h-16 w-16 md:h-24 md:w-24 rounded-full
                                    outline-4 outline-dotted outline-purple-700 dark:outline-purple-300
                                    animate-rotating duration-500 ease-out 
                                    hover:animate-none cursor-pointer">
                        </div>
                        <img    src="src/images/logo.png" 
                                class="h-16 w-16 md:h-24 md:w-24 z-20 cursor-pointer" />
                    </a>
                </div>
                <div class="flex items-start md:items-center">
                    <div
                        class=" hidden md:grid grid-cols-6 gap-x-10 
                                grow items-stretch place-content-center justify-items-center
                                px-5 max-w-7xl">
                        <a href="index.html">
                            <div class=" menu-item ">
                                Home
                            </div>
                        </a>
                        <a href="menu.html">
                            <div class="menu-item border-b-4 border-purple-400">Menu</div>
                        </a>
                        <a href="gallery.html">
                            <div class="menu-item">Gallery</div>
                        </a>
                        <a href="blogs.html"><div class="menu-item">Blogs</div></a>
                        <a href="contact_us.html"><div class="menu-item">Contact us</div></a>
                        <a href="faq.html"><div class="menu-item">FAQ</div></a>
                    </div>
                    <div class="w-5 h-5">
                        <div id="light" 
                            class="hidden cursor-pointer place-self-center" 
                            onclick="changeTheme('light')"
                            title="Normal mode">
                            <ion-icon name="sunny-outline"></ion-icon>
                        </div>
                        <div id="dark" 
                            class="cursor-pointer place-self-center" 
                            onclick="changeTheme('dark')"
                            title="Dark mode">
                            <ion-icon name="moon"></ion-icon>
                        </div>
                    </div>
                </div>
            </div>
            <aside id="drawer"
                class="  absolute top-0 z-50 bg-purple-100 text-purple-800 md:hidden
                        min-h-screen min-w-full overflow-y-hidden
                    dark:text-purple-100 dark:bg-slate-800 
                        -translate-x-[100%] duration-200 ease-in-out">
                <div class="flex flex-col py-10 px-5">
                    <div class="w-full flex justify-end">
                        <div class="w-4/6 flex justify-between">
                            <div class="relative">
                                <a href="index.html">
                                    <div
                                        class=" absolute top-0 z-10
                                                h-16 w-16 md:h-24 md:w-24 rounded-full
                                                outline-4 outline-dotted outline-purple-700 dark:outline-purple-300
                                                animate-rotating duration-500 ease-out 
                                                hover:animate-none cursor-pointer">
                                    </div>
                                    <img  src="src/images/logo.png" 
                                        class="h-16 w-16 md:h-24 md:w-24 z-20 " />
                                </a>
                            </div>
                            <div class="md:hidden" onclick="toggleMenu('close')">
                                <ion-icon size="large" name="close-outline"></ion-icon>
                            </div>
                        </div>
                    </div>
                    <ul class="flex flex-col divide-y divide-purple-200 font-jost gap-y-4 m-10 ">
                        <a href="index.html"><li class="text-base py-3">Home</li></a>
                        <a href="menu.html"><li class="text-base py-3">Menu</li></a>
                        <a href="gallery.html"><li class="text-base font-bold py-3">Gallery</li></a>
                        <a href="blogs.html"><li class="text-base py-3">Blogs</li></a>
                        <a href="contact_us.html"><li class="text-base py-3">Contact us</li></a>
                        <a href="faq.html"><li class="text-base py-3">FAQ</li></a>
                    </ul>
                </div>
            </aside>
        </header>

        <main>
            <div class="px-5 md:px-10 w-full flex flex-col bg-slate-100 dark:bg-gray-800">
                <div class="text-gray-900 text-xl md:text-3xl py-10 dark:text-slate-100">Foo...'d Eateries - for you</div>
                <div class="w-full bg-slate-100 dark:bg-gray-800 ">
                    <img class="float-left w-44 h-44 p-3" src="src/images/logo.png">
                    <p class="text-gray-700 dark:text-white clear-right first-letter:text-3xl md:first-letter:text-5xl">
                        Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes from a line in section 1.10.32.
                        The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus Bonorum et Malorum" by Cicero are also reproduced in their exact original form, accompanied by English versions from the 1914 translation by H. Rackham.
                        Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes from a line in section 1.10.32.
                        The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus Bonorum et Malorum" by Cicero are also reproduced in their exact original form, accompanied by English versions from the 1914 translation by H. Rackham.
                    </p>
                </div>
                <div class="relative">
                    <div class="z-50 inset-0 h-full w-full flex flex-col md:flex-row font-jost py-5 space-y-4 md:space-y-0 md:space-x-5">
                        <div class="w-full border border-dashed border-slate-800">
                            <div class="relative">
                                <div class="absolute -inset-0.5 bg-gradient-to-r from-pink-600 to-purple-600 blur-md opacity-75"></div>
                                <div class="relative flex flex-col">
                                    <div class="border border-slate-900 py-4 px-3 text-center text-2xl 
                                    dark:bg-slate-200 dark:text-slate-800 bg-slate-800 text-slate-300 ">
                                    South Indian
                                    </div>
                                    <div class="flex flex-col space-y-4 px-5 py-3  
                                                divide-y-2 divide-slate-200 dark:divide-slate-500
                                                text-slate-800 dark:text-slate-200
                                                bg-white dark:bg-gray-700 ">
                                        <div class="line-clamp-1 w-full pt-5">Rava idly..............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Pulao.................................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Kesaribath........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Masala Dosa........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Set Dosa.............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Rava Dosa............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Pizza Dosa.........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Idly............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Vada.................................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Sambar Vada..........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Puri..............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Upma................................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Pongal...............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Buns - Kurma........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Aloo Bonda.............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Goli Bajji.......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Rice Sambar......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">South Special Meals..........................</div>
                                        <div class="line-clamp-1 w-full pt-5">South Delux Meals.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Malbar Veg Meals.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Boiled Rice Meals..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Mini Rice Meals.....................................</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="w-full border border-dashed border-slate-800 flex flex-col">
                            <div class="relative">
                                <div class="absolute -inset-0.5 bg-gradient-to-l from-orange-600 to-sky-600 blur-md opacity-75"></div>
                                <div class="relative flex flex-col">
                                    <div class="border border-slate-900 py-4 px-3 text-center text-2xl 
                                    dark:bg-slate-200 dark:text-slate-800 bg-slate-800 text-slate-300 ">
                                    North Indian
                                    </div>
                                    <div class="flex flex-col space-y-4 px-5 py-3  
                                                divide-y-2 divide-slate-200 dark:divide-slate-500
                                                text-slate-800 dark:text-slate-200
                                                bg-white dark:bg-gray-700 ">
                                        <div class="line-clamp-1 w-full pt-5">Chole Kulcha..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Wheat Roti..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Butter Roti..............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Naan..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Veg Biriyani...................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Veg Fried Rice...................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Chapati Curry...........................</div>
                                        <div class="line-clamp-1 w-full pt-5">Parota...........................</div>
                                        <div class="line-clamp-1 w-full pt-5">Samosa.....................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Kachori...............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Masala Puri...................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Sev Puri.............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Kichdi...................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Veg Kadai...............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Aloo Fry.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Gobi Fry..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Rice Curry............................</div>
                                        <div class="line-clamp-1 w-full pt-5">North Special Meals.....................</div>
                                        <div class="line-clamp-1 w-full pt-5">North Delux Meals............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Rajasthani Veg Meals.............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Bihari Meals.............................</div>
                                        <div class="line-clamp-1 w-full pt-5">North East Special Meals......................</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="w-full border border-dashed border-slate-800 flex flex-col">
                            <div class="relative">
                                <div class="absolute -inset-0.5 bg-gradient-to-t from-amber-600 to-rose-600 blur-md opacity-75"></div>
                                <div class="relative flex flex-col">
                                    <div class="border border-slate-900 py-4 px-3 text-center text-2xl 
                                    dark:bg-slate-200 dark:text-slate-800 bg-slate-800 text-slate-300 ">
                                    Vegan
                                    </div>
                                    <div class="flex flex-col space-y-4 px-5 py-3  
                                                divide-y-2 divide-slate-200 dark:divide-slate-500
                                                text-slate-800 dark:text-slate-200
                                                bg-white dark:bg-gray-700 ">
                                        <div class="line-clamp-1 w-full pt-5">Fruits Mix....................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Veggie Masala.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Peas Bowl..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Almond-Cherry bowl...............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Coconuty.....................................</div>
                                        <div class="line-clamp-1 w-full pt-5">ChikPea curry.....................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Cashew Dosa................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Kismis Frutify.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Veg chops........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Masla Soya Paneer................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Tomato Soup...................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Mixed Veg Soup.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Fruity Poha..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Dry Fry nuts...............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Fruity Chops.............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Veg-Fruit Mix..............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Nuts Mixture..............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Vegan Meals..........................</div>
                                        <div class="line-clamp-1 w-full pt-5">Vegan Delux Meals.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Australian Vegan Bowl.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Natural Veggie..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Mini Vegan Meals.......................</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="w-full border border-dashed border-slate-800 flex flex-col">
                            <div class="relative">
                                <div class="absolute -inset-0.5 bg-gradient-to-b from-lime-600 to-indigo-600 blur-md opacity-75"></div>
                                <div class="relative flex flex-col">
                                    <div class="border border-slate-900 py-4 px-3 text-center text-2xl 
                                    dark:bg-slate-200 dark:text-slate-800 bg-slate-800 text-slate-300 ">
                                    Drinks & Juices
                                    </div>
                                    <div class="flex flex-col space-y-4 px-5 py-3  
                                                divide-y-2 divide-slate-200 dark:divide-slate-500
                                                text-slate-800 dark:text-slate-200
                                                bg-white dark:bg-gray-700 ">
                                        <div class="line-clamp-1 w-full pt-5">Tea..............................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Coffe.......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">KT........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Green Tea..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Apple Juice....................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Organge Juice..............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Mint Juice................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Cococola....................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Orange mocktail........................</div>
                                        <div class="line-clamp-1 w-full pt-5">Mixed fruit Juice.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Lemon Thunda.......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Pinaple Juice........................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Carrot Juice.......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Pupmkin Juice...........................</div>
                                        <div class="line-clamp-1 w-full pt-5">Badam Milk...............................</div>
                                        <div class="line-clamp-1 w-full pt-5">Milk n Sugar.......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Lassi......................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Buttermilk..........................</div>
                                        <div class="line-clamp-1 w-full pt-5">Clove it.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Apple Milkshake.................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Elaichi Milkshake..................................</div>
                                        <div class="line-clamp-1 w-full pt-5">Kesar Milkshare................................</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </main>
        <footer class=" static bottom-0 p-3 
                        flex justify-center bg-purple-100 
                    dark:bg-slate-800  dark:text-zinc-200">
            <div class="flex flex-col justify-center items-center">
                <img src="src/images/logo.png" class="h-12 w-12" />
                <div>Copyrights 2023</div>
                <small>Contact +91 4458156974126</small>
            </div>
        </footer>
        <script>
            let lightIcon = document.getElementById('light')
            let darkIcon = document.getElementById('dark')
            changeTheme(localStorage.theme)
            function changeTheme(theme) {
                if (theme === 'light') {
                    document.documentElement.classList.remove('dark')
                    lightIcon.classList.add("hidden");
                    darkIcon.classList.remove("hidden");
                } else if (theme === 'dark') {
                    document.documentElement.classList.add('dark')
                    lightIcon.classList.remove("hidden");
                    darkIcon.classList.add("hidden");
                }
                localStorage.setItem('theme', theme)
            }

            function toggleMenu(status) {
                let drawer = document.getElementById('drawer')
                if (status == 'open') {
                    drawer.classList.remove("-translate-x-[100%]");
                    drawer.classList.add("translate-x-0");
                } else {
                    drawer.classList.remove("translate-x-0");
                    drawer.classList.add("-translate-x-[100%]");
                }
            }


        </script>
    </body>

    </html>