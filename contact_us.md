# Contact us Page
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
                            <div class="menu-item">Blogs</div>
                        </a>
                        <a href="contact_us.html">
                            <div class="menu-item border-b-4 border-purple-400">Contact us</div>
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
                            <li class="text-base py-3">Gallery</li>
                        </a>
                        <a href="blogs.html">
                            <li class="text-base py-3">Blogs</li>
                        </a>
                        <a href="contact_us.html">
                            <li class="text-base py-3 font-bold">Contact us</li>
                        </a>
                        <a href="faq.html">
                            <li class="text-base py-3">FAQ</li>
                        </a>
                    </ul>
                </div>
            </aside>
        </header>

        <main>
            <div class="px-1 flex justify-center 
                    bg-gray-50 dark:bg-slate-800">
                <div class="w-full md:w-2/6 py-10">
                    <div class="text-center text-2xl md:text-left md:text-3xl py-5 dark:text-gray-50">Contact us</div>
                    <div class="text-center text-sm md:text-left py-2 dark:text-gray-50">Let us know you about you query</div>
                    <form method="POST" id="contact_us_form" onsubmit="return submitForm();">
                        <div class="space-y-5 my-5 px-3 md:px-0">
                            <div class="relative">
                                <input  type="text" name="fname" id="fname" autocomplete="off"
                                    class="px-4 py-2 peer w-full border border-purple-400 bg-gray-50
                                        shadow-sm placeholder-transparent text-purple-600
                                        focus:outline-none rounded-md
                                        focus:border-purple-600 focus:ring focus:ring-purple-300 focus:ring-opacity-50
                                        dark:bg-slate-800 dark:text-gray-50" placeholder="First Name" />
                                <label for="fname" class="bg-gray-50 px-2 absolute left-2 -top-3.5 text-gray-600 text-sm transition-all
                                                            peer-focus:-top-3 peer-focus:bg-gray-50
                                                        peer-focus:text-gray-600  peer-focus:text-sm
                                                            peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 
                                                            peer-placeholder-shown:top-2
                                                        dark:peer-focus:bg-slate-800 
                                                        dark:bg-slate-800  dark:text-gray-50 dark:peer-focus:text-gray-100 ">
                                                        First Name
                                </label>
                            </div>
                            <div class="relative">
                                <input  type="text" name="lname" id="lname" autocomplete="off"
                                        class="px-4 py-2 peer w-full border border-purple-400 bg-gray-50
                                            shadow-sm placeholder-transparent text-purple-600
                                            focus:outline-none rounded-md
                                            focus:border-purple-600 focus:ring focus:ring-purple-300 focus:ring-opacity-50
                                            dark:bg-slate-800 dark:text-gray-50" placeholder="Last Name" />
                                <label for="lname" class="bg-gray-50 px-2 absolute left-2 -top-3.5 text-gray-600 text-sm transition-all
                                                            peer-focus:-top-3 peer-focus:bg-gray-50
                                                        peer-focus:text-gray-600  peer-focus:text-sm
                                                            peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 
                                                            peer-placeholder-shown:top-2
                                                        dark:peer-focus:bg-slate-800 
                                                        dark:bg-slate-800  dark:text-gray-50 dark:peer-focus:text-gray-100">
                                                        Last Name
                                </label>
                            </div>
                            <div class="relative">
                                <input  type="email" name="email" id="email" autocomplete="off"
                                    class="px-4 py-2 peer w-full border border-purple-400 bg-gray-50
                                        shadow-sm placeholder-transparent text-purple-600
                                        focus:outline-none rounded-md
                                        focus:border-purple-600 focus:ring focus:ring-purple-300 focus:ring-opacity-50
                                        dark:bg-slate-800 dark:text-gray-50" placeholder="Email Address" />
                                <label for="email" class="bg-gray-50 px-2 absolute left-2 -top-3.5 text-gray-600 text-sm transition-all
                                                            peer-focus:-top-3 peer-focus:bg-gray-50
                                                        peer-focus:text-gray-600  peer-focus:text-sm
                                                            peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 
                                                            peer-placeholder-shown:top-2
                                                        dark:peer-focus:bg-slate-800 
                                                        dark:bg-slate-800  dark:text-gray-50 dark:peer-focus:text-gray-100">
                                                        Email Address
                                </label>
                                <div class="peer-invalid:mt-2 hidden peer-invalid:block text-pink-600 text-sm">
                                    Please provide a valid email address.
                                </div>
                            </div>
                            <div class="relative">
                                <input  type="number" name="mobile" id="mobile" minlength="10" autocomplete="off"
                                    class="px-4 py-2 peer w-full border border-purple-400 bg-gray-50
                                        shadow-sm placeholder-transparent text-purple-600
                                        focus:outline-none rounded-md
                                        focus:border-purple-600 focus:ring focus:ring-purple-300 focus:ring-opacity-50
                                        dark:bg-slate-800 dark:text-gray-50" placeholder="Mobile Number" />
                                <label for="mobile" class="bg-gray-50 px-2 absolute left-2 -top-3.5 text-gray-600 text-sm transition-all
                                                            peer-focus:-top-3 peer-focus:bg-gray-50
                                                        peer-focus:text-gray-600  peer-focus:text-sm
                                                            peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 
                                                            peer-placeholder-shown:top-2
                                                        dark:peer-focus:bg-slate-800 
                                                        dark:bg-slate-800  dark:text-gray-50 dark:peer-focus:text-gray-100">
                                                        Mobile Number
                                </label>
                                
                            </div>
                            <div class="relative">
                                <textarea  type="query" name="query" id="query" minlength="15" rows="10"
                                    class="px-4 py-2 peer w-full border border-purple-400 bg-gray-50
                                        shadow-sm placeholder-transparent text-purple-600
                                        focus:outline-none rounded-md
                                        focus:border-purple-600 focus:ring focus:ring-purple-300 focus:ring-opacity-50
                                        dark:bg-slate-800 dark:text-gray-50" placeholder="Type your query here"></textarea>
                                <label for="lname" class="bg-gray-50 px-2 absolute left-2 -top-3.5 text-gray-600 text-sm transition-all
                                                            peer-focus:-top-3 peer-focus:bg-gray-50
                                                        peer-focus:text-gray-600  peer-focus:text-sm
                                                            peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 
                                                            peer-placeholder-shown:top-2
                                                        dark:peer-focus:bg-slate-800 
                                                        dark:bg-slate-800  dark:text-gray-50 dark:peer-focus:text-gray-100">
                                                        Your Query
                                </label>
                            </div>
                            <div class="w-full">
                                <button type="button" onclick="submitForm(this)" class="w-full rounded-md bg-purple-600 hover:bg-purple-700 hover:shadow-md py-3 text-white">
                                    Submit
                                </button>
                            </div>
                        </div>
                    </form>
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

            function submitForm() {
                // e.preventDefault();
                alert("Submitted")
                document.getElementById('contact_us_form').reset();
            }


        </script>
    </body>

    </html>