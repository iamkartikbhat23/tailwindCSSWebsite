# Blogs page
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
                        <img src="src/images/logo.png" class="h-16 w-16 md:h-24 md:w-24 z-20 cursor-pointer" />
                    </a>
                </div>
                <div class="flex items-start md:items-center">
                    <div class=" hidden md:grid grid-cols-6 gap-x-10 
                                grow items-stretch place-content-center justify-items-center
                                px-5 max-w-7xl">
                        <a href="index.html">
                            <div class=" menu-item ">
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
                            <div class="menu-item border-b-4 border-purple-400">Blogs</div>
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
                            <div class="md:hidden" onclick="toggleMenu('close')">
                                <ion-icon size="large" name="close-outline"></ion-icon>
                            </div>
                        </div>
                    </div>
                    <ul class="flex flex-col divide-y divide-purple-200 font-jost gap-y-4 m-10 ">
                        <a href="index.html">
                            <li class="text-base py-3">Home</li>
                        </a>
                        <a href="menu.html">
                            <li class="text-base py-3">Menu</li>
                        </a>
                        <a href="gallery.html">
                            <li class="text-base">Gallery</li>
                        </a>
                        <a href="blogs.html">
                            <li class="text-base py-3 font-bold">Blogs</li>
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
            <div class=" mx-auto relative 
            bg-pink-200 dark:bg-slate-800">
                <div class="text-3xl text-center pt-10 dark:text-white drop-shadow-2xl">Blogs</div>
                <div class="  grid grid-cols-1 p-4 
                            md:grid-cols-3  
                            gap-3 place-content-stretch">
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog1.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">5 Best North Indian
                                    Recipes</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">21-08-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog2.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">3 Best South Indian
                                    Recipes</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">31-08-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog3.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Why to be Vegan</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">28-09-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog4.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Importance of best food
                                </div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">21-05-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog5.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">What to eat at what time
                                </div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">19-08-2021</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog6.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Why to be Vegan</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">16-09-2021</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog7.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Why Traditional Foods are
                                    tasty</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">23-06-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog8.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">World popular snacks
                                </div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">16-02-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog9.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Vegan: a next gen</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">29-03-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog10.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Bad food habits</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">19-09-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog11.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Tasty matters with style
                                    of Cooking</div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">14-07-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
                        </div>
                    </div>
                    <div
                        class="md:flex bg-slate-100 rounded-xl dark:bg-slate-600 min-h-max dark:border-2 dark:border-slate-50/25">
                        <img class="h-48 w-full md:w-48 md:min-h-max object-cover rounded-t-xl md:rounded-l-xl"
                            src="src/blogs/blog12.jpg" />
                        <div class="flex flex-col p-4 justify-between">
                            <div class="flex flex-col">
                                <div class="font-semibold text-lg dark:text-gray-100 line-clamp-1">Say not to food colors
                                </div>
                                <div class="text-sm text-gray-600 dark:text-gray-100 text-md line-clamp-3 md:line-clamp-4">
                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                                    when an unknown printer took a galley of type and scrambled it to
                                </div>
                            </div>
                            <div class="flex flex-col text-sm">
                                <div class="text-gray-400">12-08-2022</div>
                            </div>
                            <div
                                class="flex justify-end text-sm cursor-pointer underline text-blue-500 hover:text-blue-600">
                                Read more</div>
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