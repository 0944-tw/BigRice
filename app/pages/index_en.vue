<template>
    <div class="w-full bg-black text-center text-white py-2">
        <p>Logistics and Return Service Announcement</p>
    </div>
    <div class="w-full bg-white justify-between items-left flex px-32">
        <div class="justify-between items-left hidden md:flex ">
            <template v-for="(item) in ['Big Rice', 'Big Rice Store', 'Phones/Tablets', 'Stupid Wearables', 'Stupid Home', 'Sleeping Solutions', 'PCOC']">
                <button
                    class="ml-16 border-b-4 h-[66px] text-center  items-center flex border-transparent hover:border-b-orange-500 hover:text-orange-500">{{
                    item}}</button>
            </template>

        </div>
        <div class="hidden md:flex">
            <button
                class="ml-16 border-b-4 h-[66px] text-center  items-center flex border-transparent hover:border-b-orange-500 hover:text-orange-500">Winner List</button>
        </div>

    </div>

    <div
        class="w-full h-[600px] bg-[url(/assets/POCO_C75_MD.jpg)] md:bg-[url(/assets/POCO_C75.jpg)] bg-bottom bg-cover">
        <div class="py-32 px-4 mx-auto max-w-screen-xl  ">
            <p class="text-4xl font-bold text-center md:text-left">PCOC C75</p>
            <p class="font-bold text-center  md:text-left">The lag is real, the slowness is real</p>
            <p class="my-10 text-center  md:text-left">Starting from $114514</p>
            <div class="w-full flex justify-center md:justify-start">
                <button class="bg-black text-white px-4 py-1 rounded-xl">Order Now</button>
            </div>
        </div>
    </div>
    <div class="my-10">
        <p class="text-4xl font-bold text-center">Popular Products</p>
        <div class="justify-center items-center flex">
            <template v-for="(name) in ['Didi Baby Oil', 'Phones/Tablets', 'Genshin Impact']">
                <p
                    class="py-4 mx-2 border-b-4 border-transparent hover:border-b-orange-500 hover:text-orange-500 hover:font-semibold transition w-[92px] font-light text-center">
                    {{ name }}</p>
            </template>
        </div>
        <div class="justify-center flex my-2">
            <div class="w-full bg-white rounded-sm max-w-screen-xl">
                <!-- Xiaomi 14T Card-->
                <div class="rounded-sm h-auto md:h-[330px] w-full  m-5 max-w-screen-xl">
                    <div class="grid grid-cols-1 md:grid-cols-2">
                        <div class="overflow-hidden">
                            <img src="/assets/RandomIndiaFemalePictureXiaomi14T.jpg"
                                class="w-full h-full object-cover  hover:scale-110 transition" />
                        </div>
                        <div class="flex items-center justify-center  p-15 md:p-0 text-center">
                            <div class="text-center">
                                <p class="text-xl md:text-4xl font-bold  ">BigRice 14T Pro</p>
                                <p class="text-lg font-semibold">Save $1000 on May purchases</p>
                                <p class="text-lg font-semibold">Stack coupons to save an additional $2000</p>
                                <p class="text-lg font-extralight mt-2">Students cannot claim coupons</p>
                                <p class="text-lg font-extralight">Adults neither</p>
                                <button class="px-3 py-1 bg-black rounded-lg text-white font-bold mt-2">Not Interested</button>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Random Phone Products -->
                <div class="w-full my-5">

                    <div class="grid grid-cols-2 md:grid-cols-4 gap-5 justify-center items-center p-2">
                        <div class="bg-slate-50 p-5 rounded-xl   mx-1 text-center  " v-for="(item) in devices">
                            <div class="flex justify-center hover:scale-105 transition ease-in duration-150">
                                <img :src="item.image" class="mx-auto">
                            </div>
                            <p class="font-bold text-lg">{{ item.name }}</p>
                            <p class="font-bold text-lg mt-5"><span class="text-sm font-semibold">NT$</span>{{
                                item.price }}
                            </p>

                        </div>
                    </div>


                </div>
            </div>
        </div>

    </div>

</template>

<script setup>
const devices = ref([
    {
        name: "Remdi Pad SE 8.7",
        image: "/assets/phones/RedmiPadSE87.png",
        price: 2699
    },
    {
        name: "PCOC F6 Pro",
        image: "/assets/phones/PCOC_F6_Pro.png",
        price: 10999
    },
    {
        name: "PCOC F7 Pro",
        image: "/assets/phones/PCOC_F7_Pro.png",
        price: 14999
    },
    {
        name: "Remdi Note 14",
        image: "/assets/phones/REMDI_NOTE_14.png",
        price: 5499
    }
])

</script>