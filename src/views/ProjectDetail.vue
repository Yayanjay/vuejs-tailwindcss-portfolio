<script>
import feather from "feather-icons";
import ProjectHeader from "../components/projects/ProjectHeader.vue";

export default {
  name: "Detail",
  components: {
    ProjectHeader,
  },
  data: () => {
    return {
      singleProjectHeader: {
        singleProjectTitle: "Project Management UI",
        singleProjectDate: "Jul 26, 2021",
        singleProjectTag: "UI / Frontend",
      },
    };
  },
  mounted() {
    feather.replace();
  },
  updated() {
    feather.replace();
  },
};
</script>

<template>
  <div class="container mx-auto mt-5 sm:mt-20">
    <!-- Project header -->

    <!-- Project gallery -->
    <!-- <ProjectGallery :projectImages="projectImages" /> -->

    <!-- Project information -->
    <!-- <ProjectInfo :projectInfo="projectInfo" /> -->

    <!-- Project related projects -->
    <!-- <ProjectRelatedProjects :relatedProject="relatedProject" /> -->
    <ProjectHeader :singleProjectHeader="singleProjectHeader" />
    <!-- <section class="text-gray-600 body-font overflow-hidden"> -->
      <div class="container px-5 py-24 mx-auto">
        <div class="lg:w-4/5 mx-auto flex flex-wrap">
          <img
            alt="ecommerce"
            class="lg:w-1/2 w-full lg:h-auto h-64 object-cover object-center rounded"
            src="https://dummyimage.com/400x400"
          />
          <div class="lg:w-1/2 w-full lg:pl-10 lg:py-6 mt-6 lg:mt-0">
            <h2 class="text-sm title-font text-gray-500 tracking-widest">
              BRAND NAME
            </h2>
            <h1 class="text-gray-900 text-3xl title-font font-medium mb-1">
              The Catcher in the Rye
            </h1>
            
            <p class="leading-relaxed">
              Fam locavore kickstarter distillery. Mixtape chillwave tumeric
              sriracha taximy chia microdosing tilde DIY. XOXO fam indxgo
              juiceramps cornhole raw denim forage brooklyn. Everyday carry +1
              seitan poutine tumeric. Gastropub blue bottle austin listicle
              pour-over, neutra jean shorts keytar banjo tattooed umami
              cardigan.
            </p>
            <div class="flex space-around mt-5">
              
              <a
                href="https://github.com/Yayanjay"
                class="flex ml-auto text-white bg-purple-500 border-0 py-2 px-6 focus:outline-none hover:bg-purple-600 rounded"
                target="_blank"
              >
                Source Code
              </a>
              <a
                href="#"
                class="flex ml-auto text-white bg-purple-500 border-0 py-2 px-6 focus:outline-none hover:bg-purple-600 rounded"
              >
                Live Preview
              </a>
            </div>
          </div>
        </div>
      </div>
    <!-- </section> -->
  </div>
</template>
