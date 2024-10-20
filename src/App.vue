<router-link class="" to="/"></router-link> 
<router-view/>
  <template>
    <nav class="bg-gray-800 p-4">
      <div class="container mx-auto flex justify-between items-center">
        //logo
        <a href="#" 
        class="text-green-500 text-lg md:text2xl font-semibold">SpiceCraft</a>
        <button @click="toggleMenu" class="text-gray-400"> 
          <i class="bi bi-list text-2xl"></i>
        </button>
      </div>
    </nav>

    <div :class="menuOpen ? 'translate-x-0' : 'translate-x-full'" class="fixed top-0 right-0 w-2/3 md:w-1/4 h-full bg-gray-900 text-white transition-transform transform z-50" >
      <div class="p-4 flex justify-between items-center">
        <span class="text-green-500 text-lg font-semibold md:text-2xl"> SpiceCraft</span>
        <button @click="toggleMenu" class="text-gray-400"> 
          <i class="bi bi-x text-2xl"></i>
        </button>
      </div>
      <ul class="p-4 space-y-4">
        <li><a href="#"
          class="text-gray-300" hover:text-white >About</a>
        </li>
        <li><a href="#"
          class="text-gray-300" hover:text-white >Menu</a>
        </li>
        <li><a href="#"
          class="text-gray-300" hover:text-white >Why Choose Us</a>
        </li>
        <li><a href="#"
          class="text-gray-300" hover:text-white >Contact</a>
        </li>
      </ul>
    </div>
    <div v-if="menuOpen" @click="toggleMenu" class="fixed inset-0 bg-black opacity-50 z-40">
    </div>

    <div id="carouselExampleDark" class="carousel carousel-dark slide">
  <div class="carousel-inner">
  <div class="carousel-item active" data-bs-interval="10000">
    <img src="https://i.pinimg.com/enabled_lo/564x/84/2d/03/842d03e68c671aa86ad7a3ec54b1f2b4.jpg" class="d-block w-full h-[600px] md:h-[800px]">
    <div class="carousel-caption absolute inset-0 flex items-center justify-center text-white">
      <div class="text-center">
        <h5 class="text-4xl md:text-7xl font-bold text-green-500 ">Delicious meals</h5>
        <p class="text-2xl md:text-4xl font-bold mt-4">Savour every bite with us.</p>
        <button class="bg-green-700 h-12 md:h-20 w-40 md:w-72 md:text-4xl font-bold rounded-2xl mt-4 text-black">BOOK A TABLE.</button>
      </div>
    </div>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active" data-bs-interval="2000">
      <img src="https://i.pinimg.com/enabled_lo/564x/c8/a7/c3/c8a7c3a22a8f1e23c11bfe498146f2d6.jpg" class="d-block w-full h-[600px] md:h-[800px]">
      <div class="carousel-caption absolute inset-0 flex items-center justify-center text-white">
        <div class="text-center">
          <h5 class="text-4xl md:text-7xl font-bold text-green-400 ">Fresh ingredients</h5>
        <p class="text-2xl md:text-4xl font-bold mt-4">Hand picked just for you.</p>
        <button class="bg-green-700 h-12 md:h-20 w-40 md:w-72 md:text-4xl font-bold rounded-2xl mt-4 text-black">OUR MENU</button>
      </div>
      </div>
    </div>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item absolute inset-0 flex items-center justify-center text-white">
      <img src="https://i.pinimg.com/enabled_lo/564x/8c/28/54/8c28544c2466ca9df00d0e57dd8bba78.jpg" class="d-block w-full h-[600px] md:h-[800px]">
      <div class="carousel-caption absolute inset-0 flex items-center justify-center text-white">
        <div class="text-center">
          <h5 class="text-4xl md:text-7xl font-bold text-green-500 ">Cozy Atmosphere </h5>
        <p class="text-2xl md:text-4xl font-bold mt-4">Experience comfort and taste.</p>
        <button class="bg-green-700 h-12 md:h-20 w-40 md:w-60 md:text-4xl font-bold rounded-2xl mt-4 text-black">RESREVE NOW</button>
      </div>
      </div>
    </div>
  </div>
</div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
    <span class="carousel-control-prev-icon bg-black" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
    <span class="carousel-control-next-icon bg-black" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
<div class="container flex flex-col bg-white h-[950px] md:h-[900px] ">
      <h1 class="mt-10 text-green-500 text-3xl md:text-5xl flex justify-center">About Us</h1>
      <h1 class="text-black text-lg md:text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. At consectetur eum quidem corporis, vel suscipit voluptatem ex ut explicabo, autem recusandae dolorum! Quisquam, eligendi ullam minus consectetur voluptatem perspiciatis aperiam!</h1>
      <h1 class="text-black text-lg md:text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. At consectetur eum quidem corporis, vel suscipit voluptatem ex ut explicabo, autem recusandae dolorum! Quisquam, eligendi ullam minus consectetur voluptatem perspiciatis aperiam!</h1>
      <h1 class="text-black text-lg md:text-2xl">Lorem ipsum dolor sit amet consectetur adipisicing elit. At consectetur eum quidem corporis, vel suscipit voluptatem ex ut explicabo, autem recusandae dolorum! Quisquam, eligendi ullam minus consectetur voluptatem perspiciatis aperiam!</h1>
    <div class="flex justify-center items-center mt-5">
      <transition appear>
        <img src="https://i.pinimg.com/enabled_lo/564x/41/ca/e0/41cae02db6df0c408299a2017fa0bd41.jpg" alt="Rotating image"
        class="w-40 h-40 md:w-96 md:h-96 animate-spin-custom rounded-full "/>
      </transition>
    </div>
  </div>

    <div class="bg-gray-200">
      <div class="h-[2500px] md:h-[950px]">
      <h1 class="pt-20 flex justify-center text-green-600 md:text-5xl" >Our Menu</h1>
      <div class="md:grid md:grid-cols-3 px-8 ml-9 grid grid-cols-1">
        <div data-aos="flip-left">
        <div class=".container bg-white w-72 h-80 mt-11 rounded-lg shadow-2xl hover:shadow-green-300 flex items-center flex-col justify-center px-4">
          <i class="bi bi-cup-hot text-green-400 text-7xl"></i>
          <h1 class="text-3xl text-green-400 font-bold">Hot Beverages</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black">Explore a wide variety of  drinks to give keep you refreshed</h1>
          </div>
        </div>
        <div data-aos="flip-left">
        <div class=".container bg-white w-72 h-80 mt-11 rounded-lg shadow-2xl hover:shadow-green-300 flex items-center flex-col justify-center px-4">
          <i class="bi bi-egg-fried text-green-400 text-7xl"></i>
          <h1 class="text-3xl text-green-400 font-bold">Breakfast Special</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black"> freshly made meals to start your day right. </h1>
        </div>
        </div>
        <div data-aos="flip-left">
        <div class=".container bg-white w-72 h-80 mt-11 rounded-lg shadow-2xl hover:shadow-green-300 flex items-center flex-col justify-center px-4">
          <i class="bi bi-basket text-green-400 text-7xl"></i>
          <h1 class="text-3xl text-green-400 font-bold">Appetizers</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black"> Delicious starters to tantalise your taste buds. </h1>
        </div>
        </div>
        <div data-aos="flip-left">
        <div class=".container bg-white w-72 h-80 mt-11 rounded-lg shadow-2xl hover:shadow-green-300 flex items-center flex-col justify-center px-4">
          <i class="bi bi-check-circle-fill text-green-400 text-7xl"></i>
          <h1 class="text-3xl text-green-400 font-bold">Signature Dishes</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black"> Our chefs special creations that define our cursine. </h1>
        </div>
        </div>
        <div data-aos="flip-left">
        <div class=".container bg-white w-72 h-80 mt-11 rounded-lg shadow-2xl hover:shadow-green-300 flex items-center flex-col justify-center px-4">
          <i class="bi bi-cup-straw text-green-400 text-7xl"></i>
          <h1 class="text-3xl text-green-400 font-bold">Refreshing Drinks</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black"> Quench your thirst with our unique beverage selection. </h1>
        </div>
        </div>
        <div data-aos="flip-left">
        <div class=".container bg-white w-72 h-80 mt-11 rounded-lg shadow-2xl hover:shadow-green-300 flex items-center flex-col justify-center px-4">
          <i class="bi bi-egg text-green-400 text-7xl"></i>
          <h1 class="text-3xl text-green-400 font-bold">Desserts</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black"> Indulge in our sweet treats to end your meal on a high note. </h1>
        </div>
        </div>   
        </div>   
      </div>

      <div class="bg-white h-[1300px] md:h-[600px]">
        <div data-aos="zoom-in">
        <h1 class="pt-11 flex justify-center text-green-400 text-3xl md:text-6xl font-bold" >Why Choose Us</h1>
      </div>
      <div class="md:grid md:grid-cols-3 grid grid-cols-1 px-8" >
      <div data-aos="zoom-in">
        <div class=".container bg-gray-100 w-72 md:w-80 h-80 mt-11 rounded-lg shadow-2xl hover:border-green-300 hover:border-4  flex items-center flex-col justify-center px-2">
          <h1 class="text-3xl text-green-400 font-bold">Quality Ingedients</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black px-4"> Only the best ingredients, sourced daily. </h1>
        </div>
        </div>
      <div data-aos="zoom-in">
        <div class=".container bg-gray-100 w-72 md:w-80 h-80 mt-11 rounded-lg shadow-2xl hover:border-green-300 hover:border-4  flex items-center flex-col justify-center px-2">
          <h1 class="text-3xl text-green-400 font-bold">Friendly Service</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black px-4"> Our staff is here to make your dining experince unforgettable. </h1>
        </div>
        </div>
      <div data-aos="zoom-in">
        <div class=".container bg-gray-100 w-72 md:w-80 h-80 mt-11 rounded-lg shadow-2xl hover:border-green-300 hover:border-4  flex items-center flex-col justify-center px-2">
          <h1 class="text-3xl text-green-400 font-bold"> Cozy Ambience</h1>
          <h1 class="text-2xl md:font-medium font-bold text-black px-4">Enjoy your meal in a relaxing and welcoming environment. </h1>
        </div>
        </div>
      </div>
      </div>
    </div>
    <div data-aos="zoom-in">
    <div class=" h-[600px] md:h-[800px] bg-orange-200 flex justify-center items-center w-full" >
    <div class="w-[350px] h-[500px] md:w-[700px] md:h-[700px] bg-white shadow-lg" >
      <h1 class="text-green-400 text-3xl md:text-5xl flex justify-center font-bold mt-5">Contact Us</h1>
      <h1 class="flex justify-center text-sm md:text-2xl font-bold px-2">Feel free to reach out to us for reservations or queries.</h1>
      <div class="mt-10 ml-6 ">
      <input type="name" placeholder="Your Name" class=" border-2 border-gray-400 w-[300px] md:w-[550px] h-11 md:h-20   placeholder:text-black text-lg md:text-2xl pl-8 ">
      <input type="email" placeholder="Your Email" class="  border-2 border-gray-400 mt-3 w-[300px] md:w-[550px] h-11 md:h-20   placeholder:text-black text-lg md:text-2xl pl-8">
      <input type="message" placeholder="Your Message" class="  border-2 border-gray-400 mt-3 w-[300px] md:w-[550px] h-11 md:h-20   placeholder:text-black text-lg md:text-2xl pl-8 ">
      <button class="bg-green-600 h-12 md:h-20 w-[300px] md:w-[600px] md:text-4xl font-bold rounded-2xl text-white mt-5">Send Message</button>
    </div>
    </div>
    </div>
    <div class="bg-black w-full h-[100px] pt-3">
    <div class="flex flex-row gap-1 justify-center items-center  text-white " >
      <i class="bi bi-c-circle mt-[-8px] md:text-2xl"></i>
      <h1 class="text-sm md:text-2xl">2024</h1>
      <h1 class="text-sm md:text-2xl">SpiceCraft.</h1>
      <h1 class="text-sm md:text-2xl">All rights deserved</h1>
  </div>
  <div class="flex justify-center text-green-400 gap-2 text-2xl" >
      <i class="bi bi-facebook"></i>
      <i class="bi bi-instagram"></i>
      <i class="bi bi-twitter-x"></i>
    </div>
    </div>
    </div>
  </template>
  

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  name: 'RotatingImage',
  data () {
    return {
      menuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !
      this.menuOpen;
    },
  },
  mounted() {
    AOS.init();
  }
};
</script>

<style>
@keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.animate-spin-custom {
  animation: spin 3s linear infinite;
}

</style>

