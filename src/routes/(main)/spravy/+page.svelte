<title>Správy</title>
<body>
    
    <div class="bg-white dark:bg-gray-800 shadow xl:w-3/4 2xl:w-4/5 w-full px-6 sm:px-12 py-5 sm:py-10 mt-5 mx-auto">
        <div class="mb-5 sm:mb-10 rounded-tl-lg rounded-tr-lg">
            <div class="sm:flex items-center justify-between">
                <p  class="focus:outline-none text-base sm:text-lg md:text-xl lg:text-2xl font-bold leading-normal text-gray-800 dark:text-white ">Správy pre kontrolórov</p>
                <div class="flex items-center mt-4 sm:mt-0">
                    <div aria-label="search bar"  class="focus:outline-none focus:ring-2 focus:ring-gray-600 dark:bg-gray-800 flex items-center pl-3 bg-white border rounded-md border-gray-200 dark:border-gray-700 ">
                       <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/table_2-svg1.svg" alt="search">
                        <input type="text" class="dark:bg-gray-800 py-2.5 pl-1 w-36 sm:w-64 focus:outline-none text-sm rounded-md text-gray-600 dark:text-gray-200  placeholder-gray-400" placeholder="Vyhľadavanie" />
                    </div>
                    <button onclick="show('menu')" class="flex justify-center items-center space-x-2 ml-3 hover:ring-2 hover:ring-offset-2 hover:ring-[#98acdf] rounded">
                        <p class="text-base leading-6 dark:text-gray-100 text-gray-600">Filters</p>
                        <svg class="text-gray-600 dark:text-white" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <g clip-path="url(#clip0_159:332)">
                            <path d="M9.74926 16C9.66906 15.9999 9.58939 15.987 9.51332 15.9616L7.00863 15.1281C6.85968 15.0781 6.73029 14.9823 6.63885 14.8545C6.5474 14.7268 6.49856 14.5734 6.49926 14.4163V10.6909C6.49857 10.6894 6.49762 10.688 6.49645 10.6869L1.22613 4.54813C1.10927 4.41198 1.03393 4.24516 1.00905 4.06747C0.984179 3.88979 1.01082 3.70869 1.0858 3.54569C1.16079 3.38269 1.28097 3.24463 1.43209 3.1479C1.5832 3.05118 1.7589 2.99984 1.93832 3H15.0618C15.2412 2.99984 15.4169 3.05118 15.568 3.1479C15.7191 3.24463 15.8393 3.38269 15.9143 3.54569C15.9893 3.70869 16.0159 3.88979 15.991 4.06747C15.9662 4.24516 15.8908 4.41198 15.7739 4.54813L10.5021 10.6875C10.501 10.6888 10.5001 10.6901 10.4993 10.6916V15.25C10.4995 15.3486 10.4803 15.4462 10.4428 15.5374C10.4052 15.6285 10.3499 15.7113 10.2802 15.781C10.2105 15.8507 10.1277 15.9059 10.0366 15.9435C9.94549 15.9811 9.84783 16.0003 9.74926 16V16Z" fill="currentColor"/>
                            </g>
                            <defs>
                            <clipPath id="clip0_159:332">
                            <rect width="16" height="16" fill="white"/>
                            </clipPath>
                            </defs>
                            </svg>                        
                    </button>
                    <button onclick="popuphandler(true)" class="focus:ring-2 focus:ring-offset-2 focus:ring-[#2f52ad] inline-flex ml-5 whitespace-nowrap items-start justify-start px-6 py-3 bg-[#16254c] hover:bg-[#264187] focus:outline-none rounded">
                       <a href="novasprava"><p class="text-xs sm:text-sm font-medium leading-none text-white">Nová správa</p></a>
                    </button>
                </div>
            </div>
        </div>
        <div class="">
            <div class="w-full overflow-x-auto">
                <table class="w-full whitespace-nowrap">
                    <thead>
                        <tr class="h-20 w-full text-sm leading-none text-gray-600 dark:text-gray-200 ">
                            <th  class="focus:outline-none font-normal text-left pl-10">Názov</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Text</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Zóna</th>
                            <th  class="focus:outline-none font-normal text-left pl-10">Typ správy</th>
                            <th  class="focus:outline-none font-normal text-left pl-10 w-32">Akcie</th>
                        </tr>
                    </thead>
                    <tbody class="w-full">
                        <tr class="h-20 text-sm leading-none text-gray-700 dark:text-white  border-b border-t border-gray-200 dark:border-gray-700  bg-white dark:bg-gray-800  hover:bg-gray-100 dark:hover:bg-gray-900 ">
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <span  class="focus:outline-none">Kontak s PZ alebo s MsP</span>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">Pri akomkoľvek kontakte s príslušníkmi PZ alebo MsP, ktorý sa Vám zdá ako neštandardný je potrebné: 1.Zap...</td>
                            <td  class="focus:outline-none pl-10">Ružinov</td>
                            <td class="pl-10">
                                <div class="w-20 h-6 flex items-center justify-center bg-green-100 rounded-full">
                                    <p  class="focus:outline-none text-xs leading-3 text-green-700">Informačna</p>
                                </div>
                            </td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <button class="focus:ring-2 focus:ring-offset-2 focus:ring-[#16254c] focus:outline-none bg-gray-100 dark:bg-gray-600  mr-5 hover:bg-gray-200 dark:hover:bg-gray-900  py-2.5 px-5 rounded text-sm leading-3 text-gray-600 dark:text-gray-200 ">Upraviť</button>
                                </div>
                            </td>
                        </tr>
                        <tr class="h-20 text-sm leading-none text-gray-700 dark:text-white  border-b border-gray-200 dark:border-gray-700  bg-white dark:bg-gray-800  hover:bg-gray-100 dark:hover:bg-gray-900 ">
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <span  class="focus:outline-none">Odchody zo zmien</span>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">V zmysle nariadenia vedenia spoločnosti sú upravené zmeny nasledovne RU+SM 07:30 – 15:30 ranná zmena...</td>
                            <td  class="focus:outline-none pl-10">Všetci</td>
                            <td class="pl-10">
                                <div class="w-20 h-6 flex items-center justify-center bg-red-100 rounded-full">
                                    <p  class="focus:outline-none text-xs leading-3 text-red-700">Kritická</p>
                                </div>
                            </td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <button class="focus:ring-2 focus:ring-offset-2 focus:ring-[#16254c] focus:outline-none bg-gray-100 dark:bg-gray-600  mr-5 hover:bg-gray-200 dark:hover:bg-gray-900  py-2.5 px-5 rounded text-sm leading-3 text-gray-600 dark:text-gray-200 ">Upraviť</button>
                                </div>
                            </td>
                        </tr>
                        <tr class="h-20 text-sm leading-none text-gray-700 dark:text-white  border-b border-gray-200 dark:border-gray-700  bg-white dark:bg-gray-800  hover:bg-gray-100 dark:hover:bg-gray-900 ">
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <span  class="focus:outline-none">Striedanie zmien</span>
                                </div>
                            </td>
                            <td  class="focus:outline-none pl-10">Dnešným dňom je striedanie zmien upravené nasledovne: Kontrolór na rannej zmene vykoná uzávierku Termi...</td>
                            <td  class="focus:outline-none pl-10">Staré Mesto</td>
                            <td class="pl-10">
                                <div class="w-20 h-6 flex items-center justify-center bg-orange-100 rounded-full">
                                    <p  class="focus:outline-none text-xs leading-3 text-orange-700">Výstražna</p>
                                </div>
                            </td>
                            <td class="pl-10">
                                <div class="flex items-center">
                                    <button class="focus:ring-2 focus:ring-offset-2 focus:ring-[#16254c] focus:outline-none bg-gray-100 dark:bg-gray-600  mr-5 hover:bg-gray-200 dark:hover:bg-gray-900  py-2.5 px-5 rounded text-sm leading-3 text-gray-600 dark:text-gray-200 ">Upraviť</button>
                                </div>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>

</body>
