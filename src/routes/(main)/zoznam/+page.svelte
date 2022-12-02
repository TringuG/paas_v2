<title>Zoznam ľudí</title>
<body>
    
    <div class="bg-white dark:bg-gray-800 shadow xl:w-3/4 2xl:w-4/5 w-full px-6 sm:px-12 py-5 sm:py-10 mt-5 mx-auto">
        <div class="mb-5 sm:mb-10 rounded-tl-lg rounded-tr-lg">
            <div class="sm:flex items-center justify-between">
                <p  class="focus:outline-none text-base sm:text-lg md:text-xl lg:text-2xl font-bold leading-normal text-gray-800 dark:text-white ">Zoznam ľudí</p>
                <div class="flex items-center mt-4 sm:mt-0">
                    <div aria-label="search bar"  class="focus:outline-none focus:ring-2 focus:ring-gray-600 dark:bg-gray-800 flex items-center pl-3 bg-white border rounded-md border-gray-200 dark:border-gray-700 ">
                       <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/table_2-svg1.svg" alt="search">
                        <input type="text" class="dark:bg-gray-800 py-2.5 pl-1 w-36 sm:w-64 focus:outline-none text-sm rounded-md text-gray-600 dark:text-gray-200  placeholder-gray-400" placeholder="Vyhľadavanie" />
                    </div>
                    <button onclick="popuphandler(true)" class="focus:ring-2 focus:ring-offset-2 focus:ring-[#2f52ad] inline-flex ml-3 whitespace-nowrap items-start justify-start px-6 py-3 bg-[#16254c] hover:bg-[#264187] focus:outline-none rounded">
                       <a href="register"><p class="text-xs sm:text-sm font-medium leading-none text-white">Registrácia</p></a>
                    </button>
                </div>
            </div>
        </div>
        <div class="">
            <div class="w-full overflow-x-auto">
                <table class="w-full whitespace-nowrap">
                    <thead>
                        <tr class="h-20 w-full text-sm leading-none text-gray-600 dark:text-gray-200 ">
                            <th  class="focus:outline-none font-normal text-left pl-10">ID</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Meno</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Zóna</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Status</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Pozícia</th>
                            <th  class="focus:outline-none font-normal text-left pl-10 w-32">Akcie</th>
                        </tr>
                    </thead>
                    <tbody class="w-full">
                        <tr class="h-20 text-sm leading-none text-gray-700 dark:text-white  border-b border-t border-gray-200 dark:border-gray-700  bg-white dark:bg-gray-800  hover:bg-gray-100 dark:hover:bg-gray-900 ">
                            <td  class="focus:outline-none pl-10">133</td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <span  class="focus:outline-none">Richard Nálepka</span>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">Ružinov</td>
                            <td class="pl-10">
                                <div class="w-20 h-6 flex items-center justify-center bg-green-100 rounded-full">
                                    <p  class="focus:outline-none text-xs leading-3 text-green-700">Aktívny</p>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">Asistent</td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <button class="focus:ring-2 focus:ring-offset-2 focus:ring-[#16254c] focus:outline-none bg-gray-100 dark:bg-gray-600  mr-5 hover:bg-gray-200 dark:hover:bg-gray-900  py-2.5 px-5 rounded text-sm leading-3 text-gray-600 dark:text-gray-200 ">Zobraziť</button>
                                </div>
                            </td>
                        </tr>
                        <tr class="h-20 text-sm leading-none text-gray-700 dark:text-white  border-b border-gray-200 dark:border-gray-700  bg-white dark:bg-gray-800  hover:bg-gray-100 dark:hover:bg-gray-900 ">
                            <td  class="focus:outline-none pl-10">133</td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <span  class="focus:outline-none">Richard Nálepka</span>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">Staré Mesto</td>
                            <td class="pl-10">
                                <div class="w-20 h-6 flex items-center justify-center bg-red-100 rounded-full">
                                    <p  class="focus:outline-none text-xs leading-3 text-red-700">Neaktívny</p>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">Kontrolór</td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <button class="focus:ring-2 focus:ring-offset-2 focus:ring-[#16254c] focus:outline-none bg-gray-100 dark:bg-gray-600  mr-5 hover:bg-gray-200 dark:hover:bg-gray-900  py-2.5 px-5 rounded text-sm leading-3 text-gray-600 dark:text-gray-200 ">Zobraziť</button>
                                </div>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>

</body>

