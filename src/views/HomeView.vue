<template>
  <v-parallax height="800" src="@/images/backgroundimage.jpg">
    <div :style="overlayStyle"></div>
    <!-- Scroll Down Indicator -->
    <div class="scroll-indicator">
      <v-icon color="#15202b" size="50" @click="iconScrolldown"
        >mdi-arrow-down</v-icon
      >
    </div>
  </v-parallax>
  <v-container>
    <v-expand-x-transition>
      <v-card v-show="expand2">
        <v-row justify="end">
          <v-col cols="12" md="6" lg="4">
            <v-card class="elevation-5 pa-3 ma-5">
              <v-card-title>What is Brazilian Jiu-Jitsu?</v-card-title>
              <v-card-text>
                Brazilian Jiu-Jitsu (BJJ) is a martial art that emphasizes
                grappling and ground fighting. It's known as the "gentle art"
                because it allows a smaller person to defend themselves against
                a larger opponent using technique, leverage, and chokes or joint
                locks to gain control and force them to submit. BJJ focuses on
                taking the fight to the ground where strength is less important
                than technique. It's a great workout, builds confidence, and
                teaches self-defense skills.
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </v-expand-x-transition>

    <v-expand-x-transition>
      <v-card v-show="expand2">
        <v-row justify="start">
          <v-col cols="12" md="6" lg="4">
            <v-card class="elevation-5 pa-3 ma-5">
              <v-card-title>Why Train?</v-card-title>
              <v-card-text>
                <v-list>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Self-Defense:</v-list-item-title>
                      <v-list-item-text>
                        BJJ is a practical self-defense system that teaches you
                        to control and submit opponents regardless of size or
                        strength. It empowers people to feel confident in their
                        ability to handle themselves in a dangerous
                        situation.</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Physical Fitness:</v-list-item-title>
                      <v-list-item-text>
                        BJJ is a full-body workout that improves strength,
                        flexibility, and cardiovascular health. It's a fun and
                        challenging way to get in shape and stay
                        fit.</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Mental Toughness:</v-list-item-title>
                      <v-list-item-text>
                        BJJ teaches you to stay calm under pressure, think
                        strategically, and problem-solve in real-time. It builds
                        mental toughness and resilience that carries over into
                        other areas of your life.</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Community:</v-list-item-title>
                      <v-list-item-text>
                        BJJ is more than just a martial art; it's a community of
                        like-minded individuals who share a passion for learning
                        and growing together. It's a supportive environment
                        where you can make friends and have fun while improving
                        yourself.</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Stress Relief: </v-list-item-title>
                      <v-list-item-text>
                        BJJ is a great way to relieve stress and unwind after a
                        long day. It's a healthy outlet for pent-up energy and
                        emotions that helps you relax and
                        recharge.</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Fun: </v-list-item-title>
                      <v-list-item-text>
                        BJJ is a fun and engaging activity that challenges you
                        both mentally and physically. It's a great way to break
                        out of your comfort zone, try something new, and push
                        yourself!</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </v-expand-x-transition>

    <v-expand-x-transition>
      <v-card v-show="expand2">
        <v-row justify="end">
          <v-col cols="12" md="6" lg="4">
            <v-card class="elevation-5 pa-3 ma-5">
              <v-card-title>FAQ</v-card-title>
              <v-card-text> </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </v-expand-x-transition>

    <!--add about the coach-->
    <v-expand-x-transition>
      <v-card v-show="expand2">
        <v-row justify="center">
          <v-col cols="12" md="6" lg="4">
            <v-card class="elevation-5 pa-3 ma-5">
              <v-card-title>About the Coach</v-card-title>
              <v-card-text>
                <v-list>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Coach Name:</v-list-item-title>
                      <v-list-item-text>John Doe</v-list-item-text>
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Experience:</v-list-item-title>
                      <v-list-item-text
                        >10+ years of BJJ experience</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Rank:</v-list-item-title>
                      <v-list-item-text>Black Belt</v-list-item-text>
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Teaching Style:</v-list-item-title>
                      <v-list-item-text
                        >John is known for his patient and encouraging teaching
                        style. He breaks down techniques in a way that's easy to
                        understand and apply, making BJJ accessible to students
                        of all levels.</v-list-item-text
                      >
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </v-expand-x-transition>

    <v-card class="elevation-3">
      <v-card-title class="text-center">Time Table</v-card-title>
      <v-card class="elevation-5 pa-3 ma-5" color="green">
        <v-card-title class="font-weight-bold"
          >BJJ Beginners Class - Tuesday</v-card-title
        >
        <v-card-text class="red--text">7:30 PM - 8:30 PM</v-card-text>
        <v-card-text>
          Hull Church of Ascension
          <a
            href="https://www.google.com/maps/place/HU5+5DN"
            target="_blank"
            style="color: blue; text-decoration: underline"
            >HU5 5DN</a
          >
        </v-card-text>
        <v-card-text class="font-weight-bold">HU5 5DN</v-card-text>
      </v-card>
      <v-card class="elevation-5 pa-3 ma-5" color="green">
        <v-card-title class="font-weight-bold"
          >BJJ Beginners Class - Saturday</v-card-title
        >
        <v-card-text class="red--text">8:00 AM - 9:00 AM</v-card-text>
        <v-card-text>
          Hull Church of Ascension
          <a
            href="https://www.google.com/maps/place/HU5+5DN"
            target="_blank"
            style="color: blue; text-decoration: underline"
            >HU5 5DN</a
          >
        </v-card-text>
        <v-card-text class="font-weight-bold">HU5 5DN</v-card-text>
      </v-card>
      <v-card class="mx-auto" max-width="400">
        <v-card-title class="text-center subtitle-1">Pricing</v-card-title>
        <v-card class="elevation-8 pa-4" color="primary">
          <v-card-title class="font-weight-bold body-2 text-center"
            >Membership Options</v-card-title
          >
          <v-row>
            <v-col cols="6" class="text-center">
              <v-icon color="secondary">mdi-cash</v-icon>
              <div>Drop In</div>
              <div>£10</div>
            </v-col>
            <v-col cols="6" class="text-center">
              <v-icon color="secondary">mdi-calendar-month</v-icon>
              <div>Monthly</div>
              <div>£50</div>
            </v-col>
          </v-row>
        </v-card>
      </v-card>
    </v-card>
  </v-container>
</template>

<script>
import {
  defineComponent,
  ref,
  onMounted,
  onBeforeUnmount,
  computed,
} from "vue";

export default defineComponent({
  name: "HomeView",
  setup() {
    const expand2 = ref(false);
    const isScrolled = ref(false);
    const handleScroll = () => {
      isScrolled.value = window.scrollY > 100;
      expand2.value = true;
    };

    onMounted(() => {
      window.addEventListener("scroll", handleScroll);
    });

    onBeforeUnmount(() => {
      window.removeEventListener("scroll", handleScroll);
    });

    const overlayStyle = computed(() => ({
      position: "absolute",
      top: 0,
      left: 0,
      width: "100%",
      height: "100%",
      background: isScrolled.value ? "rgba(0, 0, 0, 0.5)" : "rgba(0, 0, 0, 0)",
    }));
    return { overlayStyle, expand2 };
  },
  methods: {
    iconScrolldown() {
      window.scrollBy(0, 2000);
    },
  },
});
</script>
<style>
.parallax-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
}
.list-background-color {
  background-color: #ffffff; /* Example: white background */
}

.scroll-indicator {
  position: absolute;
  bottom: 20px; /* Adjust based on your design */
  left: 50%;
  transform: translateX(-50%);
  animation: bounce 2s infinite;
}

@keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    transform: translateX(-50%) translateY(0);
  }
  40% {
    transform: translateX(-50%) translateY(-30px);
  }
  60% {
    transform: translateX(-50%) translateY(-15px);
  }
}
</style>
