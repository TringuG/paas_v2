<script>
	import "./app.css";

 import { onMount } from 'svelte';

let currentDateTime = new Date();

onMount(() => {
	   const interval = setInterval(() => {
		   currentDateTime = new Date();
	   }, 1000);

	   return () => {
		   clearInterval(interval);
	   };
   });

function getWeekDay(c) {
   let daysList = [
	   "Nedeľa",
	   "Pondelok",
	   "Utorok",
	   "Streda",
	   "Štvrtok",
	   "Piatok",
	   "Sobota"
   ];
   return daysList[c.getDay()];
}
function getMonth(c) {
   let monthsList = [
	   "1",
	   "2",
	   "3",
	   "4",
	   "5",
	   "6",
	   "7",
	   "8",
	   "9",
	   "10",
	   "11",
	   "12"
   ];
   return monthsList[c.getMonth()];
}
function getDate(c) {
   return c.getDate();
}
function getYear(c) {
   return c.getFullYear();
}
function getHour(c) {
   return c.getHours();
}
function getMinute(c) {
   return c.getMinutes() < 10 ? "0" + c.getMinutes() : c.getMinutes();
}
function getSeconds(c) {
   return c.getSeconds() < 10 ? "0" + c.getSeconds() : c.getSeconds();
}

</script>



<!-- UPOZORNENIE NA VRCU -->

<div>
   <div class="w-full bg-red-100 shadow rounded-md md:flex justify-between items-center">
	   <div class="sm:flex items-center">
		   <div class="flex items-end">
			   <div class="mr-2 mt-0.5 sm:mt-0 text-red-700">
				   <img class="focus:outline-none" src="https://tuk-cdn.s3.amazonaws.com/can-uploader/color-coded-with-icon-error-svg1.svg" alt="info" />
			   </div>
			   <p class="mr-2 text-base font-bold text-red-700">Informacia</p>
		   </div>
		   <div class="h-1 w-1 bg-red-700 rounded-full mr-2 hidden xl:block"></div>
		   <p class="text-base text-red-700">Web je stále vo vývoji a môžu nastať nejaké problemy. Ak nejaký problem nastane všetko hlastne na email rnalepka@raneurope.eu</p>
	   </div>
   </div>
</div>

<!-- VRCH-->

<header>
   <div class=" h-full relative">
	 <div class="bg-white border-b-2 border-[#94c356]"> 
		 <div class="2xl:container 2xl:mx-auto">
			 <nav class="">
				 <div class=" flex flex-row justify-between">
					 <div class=" flex space-x-3 items-center lg:pl-7 sm:pl-6 py-6 pl-4 pr-8">
					   <a href="teamleader"><img src="./logo.png" class="h-10 w-30" alt="logo"></a>
					 </div>
 
					 <div class="lg:flex hidden flex-auto justify-between flex-row px-7 border-l border-r border-gray-200 py-6">
					   <div class="uppercase font-sans font-bold text-[#16254c] text-2xl">
						   <span class="date">{getWeekDay(currentDateTime)} {getDate(currentDateTime)}.{getMonth(currentDateTime)}.{getYear(currentDateTime)}</span>
						   <span class="time">{getHour(currentDateTime)}:{getMinute(currentDateTime)}:{getSeconds(currentDateTime)}</span>
					   </div>
						 <div>
							<button class="border-2 border-[#94c356] rounded-lg p-2 bg-[#94c356] text-white hover:bg-[#80a84a] hover:border-[#80a84a] transition-colors duration-200 transform"><a href="teamleader" >Domov</a></button>
							 <button class="border-2 border-[#17a2b8] rounded-lg p-2 bg-[#17a2b8] text-white hover:bg-[#1490a3] hover:border-[#1490a3] transition-colors duration-200 transform"><a href="novasluzba" >Nová služba</a></button>
							 <button class="border-2 border-[#94c356] rounded-lg p-2 bg-[#94c356] text-white hover:bg-[#80a84a] hover:border-[#80a84a] transition-colors duration-200 transform"><a href="trasy" >Trasy</a></button>
							 <button class="border-2 border-[#17a2b8] rounded-lg p-2 bg-[#17a2b8] text-white hover:bg-[#1490a3] hover:border-[#1490a3] transition-colors duration-200 transform"><a href="spravy" >Správy</a></button>
							 <button class="border-2 border-[#94c356] rounded-lg p-2 bg-[#94c356] text-white hover:bg-[#80a84a] hover:border-[#80a84a] transition-colors duration-200 transform"><a href="zoznam" >Zoznam ľudí</a></button>
						   </div>  
					 </div>
					 <div class=" hidden sm:flex justify-end flex-row lg:pr-7 sm:pr-6 py-6 pr-4 pl-8">
						 <div class=" flex justify-center items-center flex-row">
							 <div class="ml-2">
								 <p class="text-lg leading-4 font-semibold text-gray-800 ">Richard Nálepka</p>
								 <p class=" font-normal text-xs leading-3 text-gray-600 mt-1">Koordinátor</p>
							 </div>
						 </div>
					 </div>

					 <div id="bgIcon" onclick="toggleMenu()"  class=" focus:outline-none focus:ring focus:ring-offset-2 focus:ring-gray-800 block sm:hidden cursor-pointer lg:pr-7 sm:pr-6 py-6 pr-4">
						 <img class="" src="https://tuk-cdn.s3.amazonaws.com/can-uploader/header-4-svg5.svg" alt="burger" />
						 <img class=" hidden" src="https://tuk-cdn.s3.amazonaws.com/can-uploader/header-4-svg6.svg" alt="cross" />                                                              
					 </div>
				 </div>
			 </nav>
		 </div>
	 </div>

	 <div id="MobileNavigation" class="hidden transform duration-150 sm:hidden h-full bg-white ">
		 <div class=" flex flex-col justify-between h-auto ">
			 <div class=" flex flex-col lg:px-7 sm:px-6 px-4">
				 <hr class=" w-full bg-gray-200 ">
				 <div class="lg:hidden flex flex-auto justify-between mt-3 flex-row pb-4">
					 <div class="">
						 <p class=" font-normal text-xs leading-3 text-gray-600 ">Hi David</p>
						 <h3 class=" font-bold text-xl leading-5 text-gray-800 mt-2">Welcome Back</h3>
					 </div>
					 <div class="cursor-pointer relative flex justify-center items-center">
						<img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/header-4-svg3.svg" alt="bell" />
						 <div class="animate-ping w-1.5 h-1.5 bg-indigo-700 rounded-full absolute top-1 right-0 m-auto duration-200"></div>
						 <div class=" w-1.5 h-1.5 bg-indigo-700 rounded-full absolute top-1 right-0 m-auto shadow-lg"></div>                                    
					 </div>
				 </div>
				 <div class=" w-auto sm:w-96 focus:outline-none focus:ring foucs:ring-offset-2 focus:ring-gray-800 bg-gray-50 flex items-center pl-4  space-x-3 rounded mt-4 ">
					 <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/header-4-svg2.svg" alt="search" />                                
					 <input aria-label="Search Bar" class=" focus:outline-none w-full bg-gray-50 font-normal pl-2 text-sm leading-4  py-3.5 text-gray-500 placeholder-gray-500 " type="text" placeholder="Search">
				 </div>
			 </div>
			 <div class=" flex items-center flex-row py-6 px-8 bg-gray-100 absolute bottom-0 left-0 w-full">
				 <img class="w-10 h-10 " src="https://i.ibb.co/QMddNDb/Ellipse-14.png" alt="Header2"/>
				 <div class="ml-2">
					 <p class="text-lg leading-4 font-semibold text-gray-800">David Hulk</p>
					 <p class=" font-normal text-xs leading-3 text-gray-600 mt-1">david@alphahulk.com</p>
				 </div>
				 <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/header-4-svg4.svg" alt="Header"/>                                    
			 </div>
		 </div>
	 </div>
 </div>
</header>


<!-- OBSAH -->

<div class="flex flex-col min-h-screen z-[50]"> 
<div class=" flex flex-1 w-full bg-[#e6ffe6] h-full">
   <div class="w-full h-full">
	   <slot />
   </div>
</div>

<!-- SPODOK -->

	 <div class="bg-[#94c356] flex justify-center p-4 overflow-hidden shadow-lg drop-shadow-xl">
	   <div class=" text-white text-center">Richard Nálepka © 2022 - 2023</div>
   </div>
</div> 