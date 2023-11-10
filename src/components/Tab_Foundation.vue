<template>
    <div class="container px-4 mx-auto">
        <div class="flex flex-wrap">
            <div class="w-full px-4 flex-1">
                <span class="text-sm block my-4 p-3 text-blueGray-700 rounded border border-solid border-blueGray-100">
                    <div class="flex flex-wrap justify-center">
                        <div class="w-6/15 sm:w-4/12 px-4">
                            <img :src="foundation1" alt="..."
                                class="shadow rounded max-w-full h-auto align-middle border-none" />
                        </div>
                        <h6 class="text-xl font-semibold mt-3">บ้านเด็กอ่อน เสือใหญ่ มูลนิธิเด็กอ่อนในสลัม</h6>
                        <p class="mt-2 mb-4 text-blueGray-400">
                            ที่อยู่: 35 177 ถนน ลาดพร้าว 23 แขวงจันทรเกษม เขตจตุจักร กรุงเทพมหานคร 10230
                        </p>

                    </div>
                    <p class="text-blueGray-500">
                        หนังสือที่ต้องการ
                    </p>
                    <p class="mb-4 text-blueGray-500">
                        - หนังสือสังคม
                    </p>
                    <div class="flex flex-wrap justify-center">
                        <button
                            class="mt-5 bg-emerald-500 text-white active:bg-emerald-600 font-bold uppercase text-sm px-6 py-3 rounded-full shadow hover:shadow-lg outline-none focus:outline-none mr-1 mb-1 ease-linear transition-all duration-150"
                            type="button">
                            Donate
                        </button>
                    </div>
                </span>
            </div>
            <div class="w-full px-4 flex-1">
                <span class="text-sm block my-4 p-3 text-blueGray-700 rounded border border-solid border-blueGray-100">
                    <div class="flex flex-wrap justify-center">
                        <div class="w-6/15 sm:w-4/12 px-4">
                            <img :src="foundation2" alt="..."
                                class="shadow rounded max-w-full h-auto align-middle border-none" />
                        </div>
                        <h6 class="text-xl font-semibold mt-3">มูลนิธิเพื่อเด็กพิการ</h6>
                        <p class="mt-2 mb-4 text-blueGray-500">
                            ที่อยู่: 546 ซอย ลาดพร้าว 47 แขวงสะพานสอง เขตวังทองหลาง กรุงเทพมหานคร 10310
                        </p>
                    </div>
                    <p class="text-blueGray-500">
                        หนังสือที่ต้องการ
                    </p>
                    <p class="mb-4 text-blueGray-500">
                        - หนังสือสังคม
                    </p>
                    <div class="flex flex-wrap justify-center">
                        <button
                            class="mt-5 bg-emerald-500 text-white active:bg-emerald-600 font-bold uppercase text-sm px-6 py-3 rounded-full shadow hover:shadow-lg outline-none focus:outline-none mr-1 mb-1 ease-linear transition-all duration-150"
                            type="button">
                            Donate
                        </button>
                    </div>
                </span>
            </div>
            <div class="w-full px-4 flex-1">
                <span class="text-sm block my-4 p-3 text-blueGray-700 rounded border border-solid border-blueGray-100">
                    <div class="flex flex-wrap justify-center">
                        <div class="w-6/15 sm:w-4/12 px-4">
                            <img :src="foundation3" alt="..."
                                class="shadow rounded max-w-full h-auto align-middle border-none" />
                        </div>
                        <h6 class="text-xl font-semibold mt-3">มูลนิธิสร้างสรรค์เด็ก</h6>
                        <p class="mt-2 mb-4 text-blueGray-500">
                            ที่อยู่: 100/475 ทุ่งสองห้อง หลักสี่ กรุงเทพมหานคร 10210
                        </p>
                    </div>
                    <p class="text-blueGray-500">
                        หนังสือที่ต้องการ
                    </p>
                    <p class="mb-4 text-blueGray-500">
                        - หนังสือสังคม
                    </p>
                    <div class="flex flex-wrap justify-center">
                        <button
                            class="mt-5 bg-emerald-500 text-white active:bg-emerald-600 font-bold uppercase text-sm px-6 py-3 rounded-full shadow hover:shadow-lg outline-none focus:outline-none mr-1 mb-1 ease-linear transition-all duration-150"
                            type="button">
                            Donate
                        </button>
                    </div>
                </span>
            </div>
        </div>
    </div>
</template>
<script>

import foundation1 from "@/assets/img/foundation1.jpg";
import foundation2 from "@/assets/img/foundation2.jpg";
import foundation3 from "@/assets/img/foundation3.jpg";

export default {
    data() {
        return {
            foundation1,
            foundation2,
            foundation3,
        }
    },
};
</script>
