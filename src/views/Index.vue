<template>
  <div>
    <index-navbar />
    <section class="header relative pt-16 items-center flex h-screen max-h-860-px">
      <div class="container mx-auto items-center flex flex-wrap">
        <div class="w-full md:w-8/12 lg:w-6/12 xl:w-6/12 px-4">
          <div class="pt-32 sm:pt-0">
            <h2 class="font-semibold text-4xl text-blueGray-600">
              Book donation system
            </h2>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-500">
              เว็บไซต์นี้จัดทำขึ้นเพื่อเป็นศูนย์รวมในการรับบริจาคหนังสือให้กับมูลนิธิหรือโรงเรียนและบุคคลที่ต้องการหนังสือ
            </p>
            <div class="mt-12">
              <a href="https://www.creative-tim.com/learning-lab/tailwind/vue/overview/notus?ref=vn-index" target="_blank"
                class="get-started text-white font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-emerald-500 active:bg-emerald-600 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150">
                Donate now
              </a>
              <a href="#scroll-target"
                class="github-star ml-1 text-white font-bold px-6 py-4 rounded outline-none focus:outline-none mr-1 mb-1 bg-blueGray-700 active:bg-blueGray-600 uppercase text-sm shadow hover:shadow-lg ease-linear transition-all duration-150"
                @click.prevent="scrollToTarget">
                View More
              </a>
            </div>
          </div>
        </div>
      </div>
      <img class="absolute top-0 b-auto right-0 pt-16 sm:w-6/12 -mt-48 sm:mt-0 w-10/12 max-h-860-px" :src="patternVue"
        alt="..." />
    </section>
    <section id="scroll-target" class="scroll-target-section bg-blueGray-200">
      <div class="header relative pt-20 items-center flex justify-center">
        <div class="flex flex-wrap">
          <div class="w-full">
            <ul class="flex mb-0 list-none flex-wrap pt-3 pb-4 flex-row">
              <li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
                <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal"
                  v-on:click="toggleTabs(1)"
                  v-bind:class="{ 'text-emerald-600 bg-white': openTab !== 1, 'text-white bg-emerald-600': openTab === 1 }">
                  <i class="fas fa-hotel text-base mr-1"></i> Foundation
                </a>
              </li>
              <li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
                <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal"
                  v-on:click="toggleTabs(2)"
                  v-bind:class="{ 'text-emerald-600 bg-white': openTab !== 2, 'text-white bg-emerald-600': openTab === 2 }">
                  <i class="fas fa-school text-base mr-1"></i> School
                </a>
              </li>
              <li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
                <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal"
                  v-on:click="toggleTabs(3)"
                  v-bind:class="{ 'text-emerald-600 bg-white': openTab !== 3, 'text-white bg-emerald-600': openTab === 3 }">
                  <i class="fas fa-users text-base mr-1"></i> Person
                </a>
              </li>
            </ul>
            <div class="relative flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded">
              <div class="px-4 py-5 flex-auto">
                <div class="tab-content tab-space">
                  <div v-bind:class="{ 'hidden': openTab !== 1, 'block': openTab === 1 }">
                    <tabFoundation />
                  </div>
                  <div v-bind:class="{ 'hidden': openTab !== 2, 'block': openTab === 2 }">
                    <tabSchool />
                  </div>
                  <div v-bind:class="{ 'hidden': openTab !== 3, 'block': openTab === 3 }">
                    <tabPerson />
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>


  </div>
</template>

<script>
import IndexNavbar from "@/components/IndexNavbar.vue";
import tabFoundation from "@/components/Tab_Foundation.vue";
import tabSchool from "@/components/Tab_School.vue";
import tabPerson from "@/components/Tab_Person.vue";
import patternVue from "@/assets/img/pattern_vue.png";

export default {
  name: "emerald-tabs",
  data() {
    return {
      patternVue,
      openTab: 1
    }
  },
  methods: {
    toggleTabs: function (tabNumber) {
      this.openTab = tabNumber
    },
    scrollToTarget: function () {
      // Replace 'scroll-target-section' with the actual class or id of the section you want to scroll to
      const targetElement = document.querySelector(".scroll-target-section");

      if (targetElement) {
        targetElement.scrollIntoView({ behavior: "smooth" });
      }
    },
  },
  components: {
    IndexNavbar,
    tabFoundation,
    tabSchool,
    tabPerson,
  },
};
</script>
