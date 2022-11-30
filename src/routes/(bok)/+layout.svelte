<script>
    import "./app.css";
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
           <p class="text-base text-red-700">Web je stále vo vývoji a môžu nastať nejaké problemy. Ak nejaký problem nastane všetko hlaste na email rnalepka@raneurope.eu</p>
       </div>
   </div>
</div>

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


