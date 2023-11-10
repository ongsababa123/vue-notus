<template>
    <div class="container px-4 mx-auto">
        <div class="flex flex-wrap">
            <div class="w-full px-4 flex-1">
                <span class="text-sm block my-4 p-3 text-blueGray-700 rounded border border-solid border-blueGray-100">
                    <div class="flex flex-wrap justify-center">
                        <div class="w-6/15 sm:w-4/12 px-4">
                            <img :src="school1" alt="..."
                                class="shadow rounded max-w-full h-auto align-middle border-none" />
                        </div>
                        <h6 class="text-xl font-semibold mt-3">วิทยาลัยการอาชีวศึกษาปทุมธานี</h6>
                        <p class="mt-2 mb-4 text-blueGray-500">
                            ที่อยู่: 2 หมู่6 ถนน รังสิต-ปทุมธานี ตำบล บางพูน อำเภอเมือง ปทุมธานี 12000
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
                            <img :src="school2" alt="..."
                                class="shadow rounded max-w-full h-auto align-middle border-none" />
                        </div>
                        <h6 class="text-xl font-semibold mt-3">มหาวิทยาลัยเทคโนโลยีพระจอมเกล้าพระนครเหนือ วิทยาเขตปราจีนบุรี
                        </h6>
                        <p class="mt-2 mb-4 text-blueGray-500">
                            ที่อยู่: Prachinburi Khao Yai, ตำบล เนินหอม Mueang, ปราจีนบุรี 25230
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
                            <img :src="school3" alt="..."
                                class="shadow rounded max-w-full h-auto align-middle border-none" />
                        </div>
                        <h6 class="text-xl font-semibold mt-3">วิทยาลัยเทคนิคปทุมธานี</h6>
                        <p class="mt-2 mb-4 text-blueGray-500">
                            ที่อยู่: เลขที่ 79 ซอย ทวีสุข หมู่ 5 ตำบล บ้านกลาง อำเภอเมืองปทุมธานี ปทุมธานี 12000
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


import school1 from "@/assets/img/school1.jpg";
import school2 from "@/assets/img/school2.jpg";
import school3 from "@/assets/img/school3.jpg";
export default {
    data() {
        return {
            school1,
            school2,
            school3,
        }
    },
};
</script>
