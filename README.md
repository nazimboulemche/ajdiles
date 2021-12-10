# Aj-Diles 
Created with HTML5 and Tailwind CSS.

## Demo 

https://user-images.githubusercontent.com/70896734/145607921-f51f4205-2a0c-4b4e-a86d-c19eea60c7aa.mp4

## Installation 
- First you need to get to the file using this command
```

cd public
```
- Then you have to install the CSS package :
```
npm install -D tailwindcss

npx tailwindcss init
```

## Usage 
- To run your page you have to click on the **index.html** file from your local files 
- **index.html** is the main page of the website

```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
  <script src="https://use.fontawesome.com/releases/v5.15.1/js/all.js" crossorigin="anonymous"></script>
  <script src="https://cdn.jsdelivr.net/gh/alpinejs/alpine@v2.x.x/dist/alpine.min.js" defer></script>
  <title>AJ Diles</title>
</head>
<style>
  #sortbox:checked~#sortboxmenu {
    opacity: 1;
  }
</style>

<body>
  <header>
    <div class="w-full text-gray-700 bg-white ">
      <div x-data="{ open: false }" class="flex flex-col max-w-screen-xl px-4 mx-auto md:items-center md:justify-between md:flex-row md:px-6 lg:px-8">
        <div class="p-4 flex flex-row items-center justify-between">
          <a href="index.html" class="text-lg font-semibold tracking-widest text-gray-900 uppercase">Logo</a>
          <button class="md:hidden rounded-lg focus:outline-none focus:shadow-outline" @click="open = !open">
            <!--CROIX-->
            <svg fill="currentColor" viewBox="0 0 20 20" class="w-6 h-6">
              <path x-show="!open" fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z" clip-rule="evenodd"></path>
              <path x-show="open" fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path>
            </svg>
          </button>
        </div>
        <nav :class="{'flex': open, 'hidden': !open}" class="flex-col flex-grow pb-4 md:pb-0 hidden md:flex md:justify-end md:flex-row">
          <div>
            <a class="px-4 py-2 mt-2 text-sm font-semibold bg-transparent rounded-lg  md:mt-0 md:ml-4 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:bg-gray-200" href="./AboutUs.html">A propos de nous</a>
            <a class="px-4 py-2 mt-2 text-sm font-semibold bg-transparent rounded-lg  md:mt-0 md:ml-4 text-white bg-red-600 hover:bg-red-700 focus:bg-red-700" href="./ContactUs.html">Contactez-nous</a>
          </div>
        </nav>
      </div>
    </div>
  </header>

  <section>
    <!--Image background-->
    <img class="max-w-lg lg:mr-20 float-right" src="./images/bg-cc3.png" alt="">
    <p class=" md:text-5xl text-4xl md:mt-15 text-red-600 text-justify  lg:text-6xl font-black pt-20 lg:pt-20 ml-52 ">AJ DILES</p>
    <p class="md:text-3xl text-xl mt-2 lg:text-3xl text-gray-800 mb-10 font-black ml-64">Consulting</p>
    <p class="font-medium ml-52 text-gray-600 mb-8">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
    <a href="" class="bg-white cursor-default select-none border-2 border-white focus:bg-white focus:text-white px-10 py-3 text-white text-lg rounded-2xl font-bold ml-52">Get started</a>
  </section>

  <!--Icons-->
  <section class="mt-6 bg-gradient-to-t from-red-200 to-white pb-16">
    <div class="flex items-center justify-evenly lg:ml-10">
      <div class="grid grid-cols-1 gap-6 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-4 xl:grid-cols-4 lg:ml-40 lg:mt-20">
        <!-- Card 1 -->
        <div class="relative bg-white py-6 px-6 rounded-3xl w-64 my-4 shadow-xl cursor-pointer ">
          <a href="#section1" class="text-white flex items-center absolute rounded-full py-4 px-4 shadow-xl bg-yellow-300 hover:bg-yellow-400 focus:bg-yellow-700 left-4 -top-6 ml-20">

            <!-- svg icon phone  -->
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-yellow-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
            </svg>
          </a>
          <div class="mt-8 ml-5">
            <div class="text-md font-semibold my-2 ml-10 cursor-pointer">Téléphonie</div>
            <div class="flex space-x-2 text-gray-400 text-sm">

            </div>
          </div>
        </div>
        <!--Card 2-->
        <div class="relative bg-white py-6 px-6 rounded-3xl w-64 my-4 shadow-xl cursor-pointer ">
          <a href="#section2" class=" text-white flex items-center absolute rounded-full py-4 px-4 shadow-xl bg-green-300 hover:bg-green-400 focus:bg-green-600 left-4 -top-6 ml-20">

            <!-- svg  icon cam-->
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-green-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z" />
            </svg>
          </a>
          <div class="mt-8 ">
            <div class="text-md font-semibold my-2  text-center cursor-pointer">Video surveillance</div>
            <div class="flex space-x-2 text-gray-400 text-sm">

            </div>
          </div>
        </div>
        <!--Card 3-->
        <div class="relative bg-white py-6 px-6 rounded-3xl w-64 my-4 shadow-xl cursor-pointer  ">
          <a href="#section3" class=" text-white flex items-center absolute rounded-full py-4 px-4 shadow-xl bg-blue-300 hover:bg-blue-400 focus:bg-blue-600 left-4 -top-6 ml-20">

            <!-- svg icon computer -->
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
          </a>
          <div class="mt-8 ml-3">
            <div+ class="text-md font-semibold my-2 ml-10 text-center cursor-pointer">Informatique</div+>
            <div class="flex space-x-2 text-gray-400 text-sm">

            </div>
          </div>
        </div>
  </section>
  <!--Téléphonie -->
  <section class="">
    <div class="" id="section1">
      <div class="flex">
        <div class="grid lg:grid-cols-2 md:grid-cols-2 bg-yellow-200 grid-flow-row-dense">
          <img class="hidden md:block " src="./images/phone.jpg">
          <div class="px-5">
            <p class="md:text-3xl lg:text-3xl text-2xl py-2  md:pt-12 md:mb-10 underline font-bold text-yellow-500">Téléphonie</p>
            <p class="md:text-lg text-gray-800 mb-5 md:mb-10 ">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit autem fugiat doloremque doloribus voluptates nemo sit corporis magni dicta asperiores inventore qui animi, provident cumque? Iusto fugiat expedita repellendus non?</p>
            <div class="mb-6">
              <a href="Telephonie.html" class="bg-white no-underline border-2  border-yellow-500 focus:bg-yellow-500 focus:text-white px-5 md:px-10 md:py-3 py-2 text-yellow-500 md:text-lg text:base rounded-lg font-bold ">En savoir plus<i class="md:text-xl text-lg md:ml-9 ml-3 focus:text-white fas fa-arrow-right"></i></a></a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Vidéo surveillance -->

    <div class="" id="section2">
      <div class="flex">
        <div class="grid lg:grid-cols-2 md:grid-cols-2 gap-4 bg-green-200 ">
          <div class="ml-10 px-5 ">
            <p class="md:text-3xl lg:text-3xl text-2xl pt-1 md:pt-12 md:mb-10 underline font-bold text-green-600">Vidéo surveillance</p>
            <p class="text-lg text-gray-800 mb-5 md:mb-10 ">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit autem fugiat doloremque doloribus voluptates nemo sit corporis magni dicta asperiores inventore qui animi, provident cumque? Iusto fugiat expedita repellendus non?</p>
            <div class="mb-6">
              <a href="VideoSurveillance.html" class="bg-white  border-2 border-green-500 focus:bg-green-600 focus:text-white px-5 md:px-10 py-2 md:py-3 text-green-500 text-lg rounded-lg font-bold ">En savoir plus<i class="md:text-xl text-lg md:ml-9 ml-3 focus:text-white fas fa-arrow-right"></i></a></a>
            </div>
          </div>
          <img class="pl-10 hidden md:block" src="./images/camera.jpg">
        </div>
      </div>
    </div>

    <!-- Informatique -->

    <div class="flex" id="section3">
      <div class="flex">
        <div class="grid lg:grid-cols-2 md:grid-cols-2 gap-4 bg-blue-300 ">
          <div class="">
            <img class="hidden md:block" src="./images/serveur.png">
          </div>
          <div class="px-5">
            <p class="md:text-3xl lg:text-3xl text-2xl pt-1  md:pt-12 md:mb-10 underline font-bold text-blue-600 ">Informatique</p>
            <p class="md:text-lg text-gray-800 mb-5 md:mb-10 ">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit autem fugiat doloremque doloribus voluptates nemo sit corporis magni dicta asperiores inventore qui animi, provident cumque? Iusto fugiat expedita repellendus non?</p>
            <div class="mb-6">
              <a href="Informatique.html" class="bg-white border-2 border-blue-500 focus:bg-blue-600 focus:text-white px-5 md:px-10 py-2 md:py-3 text-blue-500 text-lg rounded-lg font-bold ">En savoir plus<i class="md:text-xl text-lg md:ml-9 ml-3  focus:text-white fas fa-arrow-right"></i></a></a>
            </div>
          </div>
        </div>
      </div>
    </div>

  </section>

  <!--Footer-->

  <footer class=" border-t-2 border-gray-400  bg-gray-200">
    <div class="flex justify-around text-gray-700 py-5">
      <div class="space-y-2 md:my-6">
        <div class="flex">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mt-1 mr-5 text-red-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
          </svg>
          <div class="text-sm">
            <p class=" font-semibold">10 Chemin du belevédère</p>
            <p class=" font-semibold">Ormesson-sur-Marne</p>
            <p class=" font-semibold">94490</p>
          </div>
        </div>

        <div class="flex ">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mt-1 mr-5 text-red-500" viewBox="0 0 20 20" fill="currentColor">
            <path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.773a11.037 11.037 0 006.105 6.105l.774-1.548a1 1 0 011.059-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z" />
          </svg>
          <p class="py-2 font-semibold text-sm">0620114792</p>
        </div>
        <div class="flex">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mt-1 mr-5 text-red-500" viewBox="0 0 20 20" fill="currentColor">
            <path fill-rule="evenodd" d="M14.243 5.757a6 6 0 10-.986 9.284 1 1 0 111.087 1.678A8 8 0 1118 10a3 3 0 01-4.8 2.401A4 4 0 1114 10a1 1 0 102 0c0-1.537-.586-3.07-1.757-4.243zM12 10a2 2 0 10-4 0 2 2 0 004 0z" clip-rule="evenodd" />
          </svg>
          <p class="py-2 font-semibold text-sm">as@ajdiles.fr</p>
        </div>
      </div>

      <div>
        <div class="space-x-2">
          <p class="py-2 font-bold text-lg md:text-red-600 ml-2">A propos de nous</p>
          <div>
            <p class="pt-2 font-semibold hidden md:block text-sm"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. <br> Nam euismod diam vitae libero porta imperdiet. Duis vulputate et ligula ac convallis.<br>
              Sed facilisis ullamcorper odio nec luctus. Proin elementum quam arcu,<br> et pellentesque justo pharetra sit amet.
            </p>
            <a class="text-red-600 cursor-pointer font-bold underline mt-20 mr-10 text-sm" href="AboutUs.html">En savoir plus</a>

          </div>
          <a href="https://www.facebook.com/"><i class="text-3xl text-blue-800 fab fa-facebook-square"></i></a>
          <a href="https://www.linkedin.com/feed/"><i class="text-3xl text-blue-700 mt-5 fab fa-linkedin"></i></a>
        </div>
      </div>
    </div>
  </footer>
  <script src="app.js"></script>
</body>

</html>

```
- The files **styles.css** and **app.js** are required 
## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
