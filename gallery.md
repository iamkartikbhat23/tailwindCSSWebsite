# Gallery Page
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
                            <div class="menu-item">Menu</div>
                        </a>
                        <a href="gallery.html">
                            <div class="menu-item border-b-4 border-purple-400">Gallery</div>
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
            <div class=" mx-auto relative 
                    bg-teal-100 dark:bg-gray-800">
                <div class=" px-4 py-8 w-full dark:text-zinc-300
                            text-right text-xl md:text-4xl text-slate-800">
                    It's all about our ambience...
                </div>
                <div class="  grid grid-cols-2 p-4 
                            md:grid-cols-4  
                            gap-3 place-content-stretch">
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image1.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image2.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image3.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image4.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image5.jpg" 
                        alt="image"/>
                    <div class="w-full p-10 order-first col-span-2
                                md:order-none md:row-span-2 ">
                        <img class=" p-10 md:m-auto shadow-2xl shadow-emerald-600 
                                    rounded-full md:rounded" 
                            src="src/images/logo.png"
                            alt="image"/>
                    </div>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image6.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover rounded
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image7.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image8.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image9.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image10.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover rounded 
                                dark:border dark:border-gray-500" 
                        src=" src/gallery/image11.jpg" 
                        alt="image"/>
                    <img class=" inset-0 h-full w-full object-cover 
                                rounded dark:border dark:border-gray-500" 
                        src=" src/gallery/image12.jpg" 
                        alt="image"/>
                </div>
            </div>
            <div class="  relative py-20 flex flex-col space-y-8  
                        bg-sky-100 dark:bg-slate-700 overflow-hidden">
                <div class=" px-4 w-full dark:text-zinc-300 
                            text-left text-slate-800 text-xl md:text-4xl">
                    Clicks from our kitchen...
                </div>
                <div class="md:h-[18rem] grid grid-cols-2 gap-2  md:flex md:justify-between md:items-center space-x-1 md:animate-marquee ">
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/1.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/2.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/3.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/4.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/5.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/6.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/7.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/8.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/9.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/10.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/11.jpg" 
                        alt="image"/>
                    <img class="inset-0 h-full w-full object-cover " 
                        src=" src/kitchen/12.jpg" 
                        alt="image"/>
                </div>
            </div>
            <div class="p-5 bg-amber-100 dark:bg-gray-700 ">
                <div class=" px-4 py-8 w-full dark:text-zinc-300
                            text-left text-gray-700 text-xl md:text-4xl">Our food gallery...</div>
                <div class="columns-2 md:columns-5 space-y-3">
                    <img src="src/food/1.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/2.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/3.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/4.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/5.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/6.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/7.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/8.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/9.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/10.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/11.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/12.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/13.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/14.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/15.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/16.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/17.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/18.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/19.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/20.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/21.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/22.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/23.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/24.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/25.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/26.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/27.jpg"
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/28.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/29.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/30.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/31.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/32.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/33.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/34.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/35.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/36.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/37.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/38.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/39.jpg" 
                        class="rounded dark:border dark:border-amber-200">
                    <img src="src/food/40.jpg" 
                        class="rounded dark:border dark:border-amber-200">
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