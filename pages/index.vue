<template>
  <div>
    <div
      class="bg-blue-200 fixed grid grid-cols-1 rounded-md lg:grid-cols-4 gap-7 justify-content-center mt-20 mr-20 ml-20 p-8"
    >
      <div
        class="relative bg-purple-600 text-white p-8 rounded-lg lg:col-span-2"
      >
        <img
          :src="kutip"
          alt="Tanda Kutip"
          class="absolute top-8 right-14 z-0"
        />
        <CardStudent :student-data="dataStudent[0]" />
      </div>
      <div class="relative bg-gray-600 text-white p-8 rounded-lg">
        <CardStudent :student-data="dataStudent[1]" />
      </div>
      <div class="relative bg-white text-black p-8 rounded-lg lg:row-start-2">
        <CardStudent :student-data="dataStudent[2]" />
      </div>
      <div class="relative bg-black text-white p-8 rounded-lg lg:col-span-2">
        <CardStudent :student-data="dataStudent[3]" />
      </div>
      <div
        class="relative bg-white text-black p-8 rounded-lg lg:row-span-2 lg:row-start-1 lg:col-start-4"
      >
        <CardStudent :student-data="dataStudent[4]" />
      </div>
    </div>
  </div>
</template>

<script>
import CardStudent from "../components/CardStudent.vue";
export default {
  components: { CardStudent },
  data() {
    return {
      kutip: "/bg-pattern-quotation.svg",
      dataStudent: [
        {
          name: "Daniel Cliffoer",
          image: "/image-daniel.jpg",
          status: "Verified Graduated",
          quotes:
            "I received a job offer mid-course, and the subjects I learned were current, if not more so, in the company I joined. I honestly feel I got every penny’s worth.",
          opinion:
            "“ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a transition and have heard some people who had an amazing experience here. I signed up for the free intro course and found it incredibly fun! I enrolled shortly thereafter. The next 12 weeks was the best - and most grueling - time of my life. Since completing the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”",
        },
        {
          name: "Jonathan Walters",
          image: "image-jonathan.jpg",
          status: "Verified Graduated",
          quotes: "The team was very supportive and kept me motivated",
          opinion:
            "“ I started as a total newbie with virtually no coding skills. I now work as a mobile engineer for a big company. This was one of the best investments I’ve made in myself. ”",
        },
        {
          name: "Jeanette Harmon",
          image: "/image-jeanette.jpg",
          status: "Verified Graduated",
          quotes: "An overall wonderful and rewarding experience",
          opinion:
            "“ Thank you for the wonderful experience! I now have a job I really enjoy, and make a good living while doing something I love. ”",
        },
        {
          name: "Patrick Abrams",
          image: "/image-patrick.jpg",
          status: "Verified Graduated",
          quotes:
            "Awesome teaching support from TAs who did the bootcamp themselves. Getting guidance from them and learning from their experiences was easy.",
          opinion:
            "“ The staff seem genuinely concerned about my progress which I find really refreshing. The program gave me the confidence necessary to be able to go out in the world and present myself as a capable junior developer. The standard is above the rest. You will get the personal attention you need from an incredible community of smart and amazing people. ”",
        },
        {
          name: "Kira Whittle",
          image: "/image-kira.jpg",
          status: "Verified Graduated",
          quotes: "Such a life-changing experience. Highly recommended!",
          opinion:
            "“ Before joining the bootcamp, I’ve never written a line of code. I needed some structure from professionals who can help me learn programming step by step. I was encouraged to enroll by a former student of theirs who can only say wonderful things about the program. The entire curriculum and staff did not disappoint. They were very hands-on and I never had to wait long for assistance. The agile team project, in particular, was outstanding. It took my learning to the next level in a way that no tutorial could ever have. In fact, I’ve often referred to it during interviews as an example of my developent experience. It certainly helped me land a job as a full-stack developer after receiving multiple offers. 100% recommend! ”",
        },
      ],
    };
  },
};
</script>
