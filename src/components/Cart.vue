<template>
  <div class=" flex">
    <div class="  w-3/5 max-w-md mt-4 ml-20 bg-white rounded-xl shadow-md overflow-hidden md:max-w-2xl">
      <p class="mt-2 ml-5"> <strong>Cart</strong> </p>
      
  <div class="md:flex" v-for="item in products" :key="item.id">
   
    <div class="md:flex-shrink-0">
      
      <img class="h-20 w-20 object-cover rounded-lg ml-5 mt-5 mb-5" :src="item.imageUrl" :alt="item.title">
    </div>
    <div class="ml-3 mt-4">
      <div class="flex justify-between">
        <p class="text-zinc-500 flex space-x-2 text-sm">{{ item.title }}</p>
        <div class="text-black text-sm font-bold">{{ item.price }}</div>
      </div>
      <div class=" flex">
        <label class="text-zinc-400 text-xs mt-1"> {{ item.price }}</label>
        <p class="text-[#32CD32] ml-4 mt-1 text-xs"> <strong>In Stock</strong> </p>
      </div>
      <div class="flex">
        <div class="mt-3">
        <div class="shadow-sm text-zinc-500 w-15 flex items-center justify-center  rounded-md border w-20 ">
                <p class="text-xs mr-4 ml-3">{{ item.size }}</p>
                <div class="mr-2">
                  <svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" fill="currentColor" class="bi bi-caret-up-fill cursor-pointer text-xs" viewBox="0 0 16 16">
                  <path d="m7.247 4.86-4.796 5.481c-.566.647-.106 1.659.753 1.659h9.592a1 1 0 0 0 .753-1.659l-4.796-5.48a1 1 0 0 0-1.506 0z"/>
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" fill="currentColor" class="bi bi-caret-down-fill cursor-pointer text-xs" viewBox="0 0 16 16">
                <path d="M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z"/>
                </svg>
                </div>
            </div>
      </div>
      <div class="mt-3 ml-10">
        <div class="shadow-sm text-zinc-500 w-15 flex items-center justify-center  rounded-md border w-20 ">
                <p class="text-xs mr-4 ml-3">{{ item.color }}</p>
                <div class="mr-2 ">
                  <svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" fill="currentColor" class="bi bi-caret-up-fill cursor-pointer" viewBox="0 0 16 16">
                  <path d="m7.247 4.86-4.796 5.481c-.566.647-.106 1.659.753 1.659h9.592a1 1 0 0 0 .753-1.659l-4.796-5.48a1 1 0 0 0-1.506 0z"/>
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" fill="currentColor" class="bi bi-caret-down-fill cursor-pointer" viewBox="0 0 16 16">
                <path d="M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z"/>
                </svg>
                </div>
            </div>
      </div>
      
      <div class=" flex rounded ml-10 mt-3 h-7">
            <div class="text-zinc-500 w-8 flex items-center justify-center cursor-pointer rounded-l-md border-t border-l border-b">
                -
            </div>
            <div class="w-8 flex items-center  text-xs justify-center border-t border-b">1</div>
            <div class="text-zinc-500 w-8 flex items-center justify-center cursor-pointer rounded-r-md  text-s border-b border-t border-r ">+</div>
        </div>

        <div class="flex ml-12 justify-center">
      <svg  style="color: rgb(140, 140, 151);" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-heart-fill mt-3 cursor-pointer" viewBox="0 0 16 16"> <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314z" fill="#8c8c97"></path> </svg>
      <p class="text-xs ml-2 mt-3">Save</p>
    </div>
    <div class="flex ml-12 justify-center">
      <svg style="color: rgb(140, 140, 151);" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-trash-fill mt-3 cursor-pointer" viewBox="0 0 16 16"> <path d="M2.5 1a1 1 0 0 0-1 1v1a1 1 0 0 0 1 1H3v9a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V4h.5a1 1 0 0 0 1-1V2a1 1 0 0 0-1-1H10a1 1 0 0 0-1-1H7a1 1 0 0 0-1 1H2.5zm3 4a.5.5 0 0 1 .5.5v7a.5.5 0 0 1-1 0v-7a.5.5 0 0 1 .5-.5zM8 5a.5.5 0 0 1 .5.5v7a.5.5 0 0 1-1 0v-7A.5.5 0 0 1 8 5zm3 .5v7a.5.5 0 0 1-1 0v-7a.5.5 0 0 1 1 0z" fill="#8c8c97"></path> </svg>
      <p class="text-xs ml-2 mt-3 ">Delete</p>
     </div>
      </div>
      <hr class="mt-5"/>
    </div>
    
  </div>
  
</div>

<div class="max-w-md w-80 mt-4 ml-5 mr-20 bg-white rounded-xl shadow-md overflow-hidden md:max-w-2xl w-2/5">
  <div class="divide-y divide-dashed mt-5 mr-5 ml-5 mb-0">
  <div class="md:flex">
    <div>
      <p class="text-zinc-500 flex space-x-2 text-sm">Delivery</p>
      <div class="mt-2">
        <div class= " items-center h-8 flex text-zinc-500  flex  items-start justify-start  rounded-md border w-40  bg-[#EEEEEE] ">
          	<button class=" h-7 rounded-md border text-sm w-10 bg-white shadow-md ">Free</button>
            <button class="text-sm ml-3 ">Express: $9.99</button>
        </div>
        <p class="text-zinc-400 text-xs mt-2 mb-5">Delivery date: june 24, 2022 </p> 
      </div>
    </div>
  </div>
  <div>
        <div class= " items-center h-8 mt-5 flex text-zinc-500  flex justify-between rounded-md border w-70 ">
            <button class="text-sm ml-3 ">Promocode</button>
          	<button class=" h-8 rounded-md border text-sm w-12 bg-white shadow-sm "> <strong> Apply</strong></button>
        </div>
        <p class="text-zinc-400 text-xs mt-2 mb-5">20% off discount</p> 
  </div>
  <div>
    <div class="flex justify-between">
      <p class="text-zinc-500 flex space-x-2 text-sm mt-5">Subtotal</p>
      <p class="text-zinc-500 flex space-x-2 text-xs mt-5">$80.96</p>
    </div>
    <div class="flex justify-between">
      <p class="text-zinc-500 flex space-x-2 text-xs mt-3">Discount</p>
      <p class="text-zinc-500 flex space-x-2 text-xs mt-3">(20%) - $16.19</p>
    </div>
    <div class="flex justify-between">
      <div class="flex">
        <p class="text-zinc-500 flex space-x-2 text-xs mt-3">Delivery</p>
        <i class="fa-solid fa-circle-info fa-xs mt-5 ml-1" style="color: #a6adb9;"></i>
      </div>
      <p class="text-zinc-500 flex space-x-2 text-xs mt-3">$0.00</p>
    </div>
    <div class="flex justify-between mb-5">
      <div class="flex">
        <p class="text-zinc-500 flex space-x-2 text-xs mt-3">Tax</p>
        <i class="fa-solid fa-circle-info fa-xs mt-5 ml-1" style="color: #a6adb9;"></i>
      </div>
      <p class="text-zinc-500 flex space-x-2 text-xs mt-3">+$14.00</p>
    </div>
  </div>
  <div class="flex justify-between ">
      <p class="text-zinc-500 flex space-x-2 text-sm mt-5">Total</p>
      <p class="text-zinc-500 flex space-x-2 text-xs mt-5">$78.76</p>   
  </div>      
</div>
            <button class=" p-2 items-center  mt-3 m-auto ml-16 sm:mr-16  bg-blue-500 hover:bg-blue-700 text-white rounded-md  ">Proceed to checkout</button>
            <button class=" p-2 pr-4 items-center  mt-2 m-auto ml-16 sm:mr-16  border border-blue-500 hover:bg-blue-100 text-blue-700 rounded-md  ">Continue shopping</button>
      
  </div>
</div>
 
  </template>
 
<script>
import products from '../mock/products.json';
 export default{
   name:"ProductList",
   data(){
    return{
      products,
    }
   }
   }
</script>

