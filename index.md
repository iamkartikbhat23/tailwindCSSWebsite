# Index page or Home Page
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
        <link href="https://fonts.googleapis.com/css2?family=Domine:wght@500&family=Jost:wght@500&display=swap"
            rel="stylesheet">

    </head>

    <body class="font-domine">

        <header class=" sticky top-0 z-20
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
                        <div class=" absolute top-0 z-10
                                    h-16 w-16 md:h-24 md:w-24 rounded-full
                                    outline-4 outline-dotted outline-purple-700 dark:outline-purple-300
                                    animate-rotating duration-500 ease-out 
                                    hover:animate-none cursor-pointer">
                        </div>
                        <img src="src/images/logo.png" class="h-16 w-16 md:h-24 md:w-24 z-20 " />
                    </a>
                </div>
                <div class="flex items-start md:items-center">
                    <div class=" hidden md:grid grid-cols-6 gap-x-10 
                                grow items-stretch place-content-center justify-items-center
                                px-5 max-w-7xl">
                        <a href="index.html">
                            <div class=" menu-item border-b-4 border-purple-400">
                                Home
                            </div>
                        </a>
                        <a href="menu.html">
                            <div class="menu-item">Menu</div>
                        </a>
                        <a href="gallery.html">
                            <div class="menu-item">Gallery</div>
                        </a>
                        <a href="blogs.html">
                            <div class="menu-item">Blogs</div>
                        </a>
                        <a href="contact_us.html">
                            <div class="menu-item">Contact us</div>
                        </a>
                        <a href="faq.html">
                            <div class="menu-item">FAQ</div>
                        </a>
                    </div>
                    <div class="w-5 h-5">
                        <div id="light" class="hidden cursor-pointer place-self-center" onclick="changeTheme('light')"
                            title="Normal mode">
                            <ion-icon name="sunny-outline"></ion-icon>
                        </div>
                        <div id="dark" class="cursor-pointer place-self-center" onclick="changeTheme('dark')"
                            title="Dark mode">
                            <ion-icon name="moon"></ion-icon>
                        </div>
                    </div>
                </div>
            </div>
            <aside id="drawer" class="  absolute top-0 z-50 bg-purple-100 text-purple-800 md:hidden
                        min-h-screen min-w-full overflow-y-hidden
                    dark:text-purple-100 dark:bg-slate-800 
                        -translate-x-[100%] duration-200 ease-in-out">
                <div class="flex flex-col py-10 px-5">
                    <div class="w-full flex justify-end">
                        <div class="w-4/6 flex justify-between">
                            <div class="relative">
                                <div class=" absolute top-0 h-16 w-16 md:h-24 md:w-24 rounded-full 
                                            outline-4 outline-dotted outline-purple-700 dark:outline-purple-300
                                            animate-rotating duration-500 ease-out">
                                </div>
                                <a href="index.html">
                                    <img src="src/images/logo.png" class="h-16 w-16 md:h-24 md:w-24 z-20" />
                                </a>
                            </div>
                            <div class="md:hidden" onclick="toggleMenu('close')">
                                <ion-icon size="large" name="close-outline"></ion-icon>
                            </div>
                        </div>
                    </div>
                    <ul class="flex flex-col divide-y divide-purple-200 font-jost gap-y-4 m-10 ">
                        <a href="index.html">
                            <li class="text-base font-bold py-3">Home</li>
                        </a>
                        <a href="menu.html">
                            <li class="text-base py-3">Menu</li>
                        </a>
                        <a href="gallery.html">
                            <li class="text-base py-3">Gallery</li>
                        </a>
                        <a href="blogs.html">
                            <li class="text-base py-3">Blogs</li>
                        </a>
                        <a href="contact_us.html">
                            <li class="text-base py-3">Contact us</li>
                        </a>
                        <a href="faq.html">
                            <li class="text-base py-3">FAQ</li>
                        </a>
                    </ul>
                </div>
            </aside>
        </header>

        <main>
            <div class="relative p-3 md:p-10 min-h-screen max-w-screen 
                        bg-[url('https://images.pexels.com/photos/326333/pexels-photo-326333.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]  
                        dark:contrast-125">
                <div class="    grid grid-cols-1 md:grid-cols-2 grid-rows-2 
                                items-stretch place-content-center min-h-screen 
                                text-white text-3xl">
                    <div class=" border md:border-l-4 md:border-y-4 border-sky-400 md:rounded-tl-xl 
                            dark:border-stone-300">
                        <div class="h-full py-10 flex flex-col justify-center items-center">
                            South Indian
                            <img src="src/images/sf.png" class="h-44 w-44 md:h-80 md:w-80" />
                        </div>
                    </div>
                    <div class="  border md:border-t-4 md:border-x-4 border-amber-500 md:rounded-tr-xl 
                                dark:border-stone-300">
                        <div class="h-full py-10 flex flex-col justify-center items-center">
                            North Indian
                            <img src="src/images/nf.png" class="h-44 w-44 md:h-80 md:w-80" />
                        </div>
                    </div>
                    <div class=" border md:border-b-4 md:border-x-4 border-blue-600 md:rounded-bl-xl
                            dark:border-stone-300">
                        <div class="h-full py-10 flex flex-col justify-center items-center">
                            Vegan
                            <img src="src/images/vf.png" class="h-44 w-44 md:h-80 md:w-80" />
                        </div>
                    </div>
                    <div class=" border md:border-r-4 md:border-y-4 border-orange-600 md:rounded-br-xl 
                            dark:border-stone-300">
                        <div class="h-full py-10 flex flex-col justify-center items-center">
                            Drinks and Juices
                            <img src="src/images/juices.png" class="h-44 w-44 md:h-80 md:w-80" />
                        </div>
                    </div>
                </div>
                <div class=" hidden absolute top-0 h-full w-[95%] z-10
                            md:flex items-center justify-center">
                    <img src="src/images/logo.png" class=" h-44 w-44 drop-shadow-2xl cursor-pointer 
                                border-2 border-dashed border-zinc-200 rounded-full 
                                hover:animate-waving duration-900 ease-in-out" />
                </div>
            </div>
            <div class=" h-full w-full md:h-[20rem] p-10 font-jost 
                    bg-lime-200  flex justify-center 
                    dark:bg-slate-800/90 text-gray-800 dark:text-white">
                <div class="w-full flex flex-col md:flex-row justify-around text-2xl">
                    <div class="px-20 flex flex-col items-center justify-center">
                        <lord-icon src="https://cdn.lordicon.com/vukdchss.json" trigger="loop" delay="2000"
                            class="h-36 w-36 md:h-[10rem] md:w-[10rem]">
                        </lord-icon>
                        <div class="font-semibold">Clean</div>
                    </div>
                    <div class=" px-20 flex flex-col items-center justify-center">
                        <lord-icon src="https://cdn.lordicon.com/ihyatngg.json" trigger="loop" delay="2000"
                            class="h-36 w-36 md:h-[10rem] md:w-[10rem]">
                        </lord-icon>
                        <div class="font-semibold">Quality</div>
                    </div>
                    <div class="px-20 flex flex-col items-center justify-center">
                        <lord-icon src="https://cdn.lordicon.com/efdhjqgx.json" trigger="loop" delay="2000"
                            class="h-36 w-36 md:h-[10rem] md:w-[10rem]">
                        </lord-icon>
                        <div class="font-semibold">Original</div>
                    </div>
                </div>
            </div>
            <div class="  container min-w-full p-2 md:p-10 
                        bg-orange-200 dark:bg-slate-600 ">
                <div class="  flex justify-center text-4xl py-3 font-semibold font-jost 
                            text-gray-700  dark:text-zinc-200">
                    Reviews
                </div>
                <div class=" columns-1 px-4 text-xs p-5 space-y-3
                            md:columns-3 md:px-10 md:text-base 
                        dark:text-zinc-200 shadow-inner">
                    <div class=" flex flex-col p-4 
                                border border-secondary rounded-md 
                            dark:bg-slate-800 ">
                        <div class="flex space-x-2 items-center">
                            <img src="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=4&w=256&h=256&q=80"
                                class="w-12 h-12 rounded-full" />
                            <div class="text-md font-semibold">Person 1</div>
                        </div>
                        <div class="italic">
                            Nice ambience, good restaurant
                        </div>
                    </div>
                    <div class=" flex flex-col p-4 
                                border border-primary rounded-md 
                            dark:bg-slate-800 ">
                        <div class="flex space-x-2 items-center">
                            <img src="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=4&w=256&h=256&q=80"
                                class="w-12 h-12 rounded-full" />
                            <div class="text-md font-semibold">Person 2</div>
                        </div>
                        <div class="italic">
                            Good Taste :)
                        </div>
                    </div>
                    <div class=" flex flex-col p-4 
                                border border-tertiary rounded-md 
                            dark:bg-slate-800 ">
                        <div class="flex space-x-2 items-center">
                            <img src="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=4&w=256&h=256&q=80"
                                class="w-12 h-12 rounded-full" />
                            <div class="text-md font-semibold">Person 3</div>
                        </div>
                        <div class="italic">
                            Pocket friendly prices.. best offers
                        </div>
                    </div>
                    <div class=" flex flex-col p-4 
                                border border-quaternary rounded-md 
                                dark:bg-slate-800 ">
                        <div class="flex space-x-2 items-center">
                            <img src="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=4&w=256&h=256&q=80"
                                class="w-12 h-12 rounded-full" />
                            <div class="text-md font-semibold">Person 4</div>
                        </div>
                        <div class="italic">
                            Decent Environment, lots of choices
                        </div>
                    </div>
                    <div class="  flex flex-col p-4 
                                border border-quinary rounded-md 
                                dark:bg-slate-800 ">
                        <div class="flex space-x-2 items-center">
                            <img src="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=4&w=256&h=256&q=80"
                                class="w-12 h-12 rounded-full" />
                            <div class="text-md font-semibold">Person 5</div>
                        </div>
                        <div class="italic">
                            Overall Good Experience
                        </div>
                    </div>
                    <div class=" flex flex-col p-4 
                                border border-secondary rounded-md 
                            dark:bg-slate-800 ">
                        <div class="flex space-x-2 items-center">
                            <img src="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=facearea&facepad=4&w=256&h=256&q=80"
                                class="w-12 h-12 rounded-full" />
                            <div class="text-md font-semibold">Person 6</div>
                        </div>
                        <div class="italic">
                            Nice Restaurant with good, clean maintenance
                        </div>
                    </div>
                </div>
            </div>
            <div class="  container min-w-full p-10 
                        bg-rose-200 dark:bg-gray-800">
                <div class="flex flex-col md:flex-row justify-around gap-y-6">
                    <div class=" w-full md:w-44 lg:w-56 xl:w-72 2xl:w-80 flex flex-col p-5 
                                text-center text-gray-700 dark:text-gray-200 
                                border border-rose-500 rounded-md shadow-xl shadow-rose-400
                            dark:border-gray-100  dark:shadow-gray-100 dark:hover:border-gray-50
                                hover:-translate-y-5 duration-150 hover:border-rose-700 hover:shadow-2xl">
                        <div class="text-2xl">400+</div>
                        <div class="text-base">Tables</div>
                    </div>
                    <div class=" w-full md:w-44 lg:w-56 xl:w-72 2xl:w-80 flex flex-col p-5 
                                text-center text-gray-700 dark:text-gray-200 
                                border border-rose-500 rounded-md shadow-xl shadow-rose-400
                            dark:border-gray-100  dark:shadow-gray-100 dark:hover:border-gray-50
                                hover:-translate-y-5 duration-150 hover:border-rose-700 hover:shadow-2xl">
                        <div class="text-2xl">500+</div>
                        <div class="text-base">Dishes</div>
                    </div>
                    <div class=" w-full md:w-44 lg:w-56 xl:w-72 2xl:w-80 flex flex-col p-5 
                                text-center text-gray-700 dark:text-gray-200 
                                border border-rose-500 rounded-md shadow-xl shadow-rose-400
                            dark:border-gray-100  dark:shadow-gray-100 dark:hover:border-gray-50
                                hover:-translate-y-5 duration-150 hover:border-rose-700 hover:shadow-2xl">
                        <div class="text-2xl">10-15 Mins</div>
                        <div class="text-base">Prep. Time</div>
                    </div>
                    <div class=" w-full md:w-44 lg:w-56 xl:w-72 2xl:w-80 flex flex-col p-5 
                                text-center text-gray-700 dark:text-gray-200 
                                border border-rose-500 rounded-md shadow-xl shadow-rose-400
                            dark:border-gray-100  dark:shadow-gray-100 dark:hover:border-gray-50
                                hover:-translate-y-5 duration-150 hover:border-rose-700 hover:shadow-2xl">
                        <div class="text-2xl">25</div>
                        <div class="text-base">Total Kitchens</div>
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