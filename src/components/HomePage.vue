<template>
  <div>
    <!-- First Parallex -->
    <section id ="home">
      <v-parallax :src="getImageUrl('banner.jpg')" height="680" alt="banner image">
        <v-layout column align-center justify-center class="white--text">
          <img :src="getImageUrl('logo.png')" alt="Hackathon Logo" height="300">
          <h3 class="display-1 text-xs-center">U.S Embassy in Ethiopia presents</h3>
          <h3 class="white--text font-weight-bold mb-2 display-2 text-xs-center">Hackathon <span class="display-1">v2.0</span></h3>
          <div class="title mb-4 text-xs-center">From Jan 11-13, 2018</div>
          <div class="subheading mb-3 text-xs-center">@ American Center, Addis Ababa</div>
          <v-btn class="blue lighten-2 mt-5" dark large href="https://goo.gl/HEa1i6">Register Here</v-btn>
        </v-layout>
      </v-parallax>
    </section>

    <!-- Featured Text -->
    <section id ="why">
      <v-layout column wrap class="my-5" align-center>
        <v-flex xs12 sm4 class="my-3">
          <div class="text-xs-center">
            <h2 class="headline">The best way to demonistrate your coding skill</h2>
            <span class="subheading">while solving potential problems</span>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <v-icon x-large class="blue--text text--lighten-2">color_lens</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-xs-center">Design The Challenge</div>
                  </v-card-title>
                  <v-card-text>
                    Hackathon boosts your design skill and critical thinking towards solving the challenge. It give you the opportunity to improve your
                    skill on how to understand the problem domain or the challenge topic, analze and come up with potential
                    ,feasible solution.
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <v-icon x-large class="blue--text text--lighten-2">build</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline">Build The Solution</div>
                  </v-card-title>
                  <v-card-text>
                    You will build digital solution that trully solves the problem. By collaboration with a team, you
                    will learn how to coordinate to build the designed solution. You will demonistrate your skill
                    within a short period of time. You will also learn new skills from the teams.
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <v-icon x-large class="blue--text text--lighten-2">flash_on</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-xs-center">Win Big Prizes</div>
                  </v-card-title>
                  <v-card-text>
                    You will get big prizes for your outstanding solution/product. You will also get exposure to the
                    potential stakeholders to work on the winning project. This award is a complement for your passion.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Second Parallex -->
    <section>
      <v-parallax :src="getImageUrl('hacking.jpg')" height="380">
        <v-layout column align-center justify-center>
          <!-- <div
            class="headline white--text mb-3 text-xs-center"
          >Web development has never been easier</div>-->
          <em>“Whether we're fighting climate change or going to space,
            <br>everything is moved forward by computers, and we don't
            <br>have enough people who can code.”
            <br>- Richard Branson
          </em>
        </v-layout>
      </v-parallax>
    </section>

    <!-- Organizors -->
    <section id="about">
      <v-layout column wrap class="my-5" align-center>
        <v-flex xs12 sm4 class="my-3">
          <div class="text-xs-center">
            <h2 class="headline font-weight-medium">Organized by U.S Embassy in Ethiopia</h2>
            <span class="subheading">#USInvestsInEthiopians</span><br/>
            <a href="https://et.usembassy.gov/nofo-for-ethiopia-hacks/" target="blank">NOFO for Ethiopia Hacks</a>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12 md3>
                <v-card target="blank" href="https://et.usembassy.gov/" class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <img :src="getImageUrl('us_embassy.png')" alt="Hackathon Logo" height="150">
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="subheading text-xs-center">U.S. Embassy</div>
                  </v-card-title>
                </v-card>
              </v-flex>

              <v-flex xs12 md3>
                <v-card class="elevation-0 transparent" href="https://www.usaid.gov/ethiopia" target="blank">
                  <v-card-text class="text-xs-center">
                    <img :src="getImageUrl('usaid.png')" alt="Hackathon Logo" height="150">
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="subheading text-xs-center">USAID</div>
                  </v-card-title>
                </v-card>
              </v-flex>

              <v-flex xs12 md3>
                <v-card class="elevation-0 transparent" href="https://www.meetup.com/GDG-Addis" target="blank">
                  <v-card-text class="text-xs-center">
                    <img :src="getImageUrl('new_gdgaddis_logo.jpg')" alt="Hackathon Logo" height="150">
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="subheading text-xs-center">GDG Addis</div>
                  </v-card-title>
                </v-card>
              </v-flex>

              <v-flex xs12 md3>
                <v-card class="elevation-0 transparent" href="http://cawee-ethiopia.com/" target="blank">
                  <v-card-text class="text-xs-center">
                    <img :src="getImageUrl('cawee.png')" alt="Hackathon Logo" height="150">
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="subheading text-xs-center">CAWEE</div>
                  </v-card-title>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Time Line -->
    <section id="timeline">
      <v-layout column align-center>
        <v-flex xs12 md6>
          <v-timeline>
            <v-timeline-item color="purple lighten-2" fill-dot right>
              <v-card>
                <v-card-title class="purple lighten-2">
                  <v-icon dark size="42" class="mr-3">mdi-magnify</v-icon>
                  <h2 class="display-1 white--text font-weight-light">Hackathon v1.0</h2>
                </v-card-title>
                <v-container>
                  <v-layout>
                    <v-flex xs10>
                      <p>"Entreprunership and youth"</p>
                      <p>Nov 16 to 18, 2018 at American Center, Addis Ababa.</p>
                    </v-flex>
                    <v-flex xs2>
                      <v-icon size="64">mdi-calendar-text</v-icon>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-card>
            </v-timeline-item>

            <v-timeline-item color="amber lighten-1" fill-dot left small>
              <v-card>
                <v-card-title class="amber lighten-1 justify-end">
                  <h2 class="display-1 mr-3 white--text font-weight-light">Hackathon v2.0</h2>
                  <v-icon dark size="42">mdi-home-outline</v-icon>
                </v-card-title>
                <v-container>
                  <v-layout>
                    <v-flex xs12>
                      <p>"comming soon.."</p>
                      <p>Jan 11 to 13, 2019 at American Center, Addis Ababa.</p>
                      <v-btn
                        class="blue lighten-2 mt-5"
                        dark
                        
                        href="https://goo.gl/HEa1i6"
                      >Register Here</v-btn>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-card>
            </v-timeline-item>

            <v-timeline-item color="cyan lighten-1" fill-dot right>
              <v-card>
                <v-card-title class="cyan lighten-1">
                  <v-icon class="mr-3" dark size="42">mdi-email-outline</v-icon>
                  <h2 class="display-1 white--text font-weight-light">Hackathon v3.0</h2>
                </v-card-title>
                <v-container>
                  <v-layout>
                    <v-flex xs12>
                      <p>Comming Soon...</p>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-card>
            </v-timeline-item>

            <v-timeline-item color="red lighten-1" fill-dot left small>
              <v-card>
                <v-card-title class="red lighten-1 justify-end">
                  <h2 class="display-1 mr-3 white--text font-weight-light">Hackathon v4.0</h2>
                  <v-icon dark size="42">mdi-account-multiple-outline</v-icon>
                </v-card-title>
                <v-container>
                  <v-layout>
                    <v-flex xs2>
                      <v-icon size="64">mdi-server-network</v-icon>
                    </v-flex>
                    <v-flex xs10>
                      <p>Comming Soon...</p>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-card>
            </v-timeline-item>

            <v-timeline-item color="green lighten-1" fill-dot right>
              <v-card>
                <v-card-title class="green lighten-1">
                  <v-icon class="mr-3" dark size="42">mdi-phone-in-talk</v-icon>
                  <h2 class="display-1 white--text font-weight-light">Hackathon v5.0</h2>
                </v-card-title>
                <v-container>
                  <v-layout>
                    <v-flex>
                      <p>Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.</p>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-card>
            </v-timeline-item>
          </v-timeline>
        </v-flex>
      </v-layout>
    </section>

    

    <!-- FAQ -->
    <section id="faq">
      <v-layout column align-center>
        <h4 class="display-1">FAQ</h4>
      </v-layout>
      <v-layout row wrap>
        <v-flex xs12 md6 lg6 v-for="(faq, key) in faqList" :key="key">
          <v-expansion-panel popout>
            <v-expansion-panel-content>
              <v-layout slot="header" align-center row spacer>
                <v-flex no-wrap xs15>
                  <p>{{faq.question}}</p>
                </v-flex>
              </v-layout>
              <v-card>
                <v-divider></v-divider>
                <v-card-text v-text="faq.answer"></v-card-text>
              </v-card>
            </v-expansion-panel-content>
          </v-expansion-panel>
        </v-flex>

      </v-layout>
    </section>

    <!-- Contact -->
    <section id = "contact">
      <v-container grid-list-xl>
        <v-layout row wrap justify-center class="my-5">
          <v-flex xs12 sm4>
            <v-card class="elevation-0 transparent">
              <v-card-title primary-title class="layout justify-center">
                <div class="headline">Program Objective</div>
              </v-card-title>
              <v-card-text>
                Ethiopia is the second most-populous country in Africa with more than 70% of its population
                under the age of 35. This population of youth faces enormous challenges in terms of education,
                employment, access to technology and opportunities to create and innovate.
                Hackathon participants are between the of 18-25 thus hosting a Hackathon allows to understand
                how best to inspire Ethiopian youth to imagine, plan, design, compose, invent, create, innovate,
                build and construct. The program aims to make the most diverse hackathon sessions with a goal
                of 35% participation from women in each session.
              </v-card-text>
            </v-card>
          </v-flex>
          <v-flex xs12 sm4 offset-sm1>
            <v-card class="elevation-0 transparent">
              <v-card-title primary-title class="layout justify-center">
                <div class="headline">Contact us</div>
              </v-card-title>
              <v-card-text>Do you want to contact the organizers? Please don't hesitate to contact through the following addresses.</v-card-text>
              <v-list class="transparent">
                <v-list-tile>
                  <v-list-tile-action>
                    <v-icon class="blue--text text--lighten-2">phone</v-icon>
                  </v-list-tile-action>
                  <v-list-tile-content>
                    <v-list-tile-title>+251-910331122</v-list-tile-title>
                  </v-list-tile-content>
                </v-list-tile>
                <v-list-tile>
                  <v-list-tile-action>
                    <v-icon class="blue--text text--lighten-2">place</v-icon>
                  </v-list-tile-action>
                  <v-list-tile-content>
                    <v-list-tile-title>American Centers in Ethiopia</v-list-tile-title>
                  </v-list-tile-content>
                </v-list-tile>
                <v-list-tile>
                  <v-list-tile-action>
                    <v-icon class="blue--text text--lighten-2">email</v-icon>
                  </v-list-tile-action>
                  <v-list-tile-content>
                    <v-list-tile-title>gdgaddis.et@gmail.com</v-list-tile-title>
                  </v-list-tile-content>
                </v-list-tile>
              </v-list>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </section>
  </div>
</template>


<script>

import * as easings from 'vuetify/es5/util/easing-patterns'

export default {
  
  data() {
    return {
      title: '"Ethiopia Hacks" Hackathon v2.0',
      messages: [
        {
          avatar: "https://avatars0.githubusercontent.com/u/9064066?v=4&s=460",
          name: "Melake Wubshet",
          title: "Welcome to Vuetify.js!",
          excerpt: "Thank you for joining our community..."
        },
        {
          color: "red",
          icon: "people",
          name: "Social",
          new: 1,
          total: 3,
          title: "Twitter"
        },
        {
          color: "teal",
          icon: "local_offer",
          name: "Promos",
          new: 2,
          total: 4,
          title: "Shop your way",
          exceprt: "New deals available, Join Today"
        }
      ],
      
       faqList: [
        {
          question: 'What is Hackathon?',
          answer: 'A hackathon is usually a day long (can be 36 hours, 48 hours, etc.) coding competition where software programmers, developers, designers, etc. come together to build and design something cool.'
        },
        {
          question: 'Who can attend ‘Ethiopia Hack’ hackathon??',
          answer: 'Anyone who is interested in computer programming and loves to learn and build cool stuff can attend.'
        },
        {
          question: 'But isn’t hacking illegal? ',
          answer: 'The word “hack” has so much negativity attached to it that most people think hackathons are a way to “hack” into something. NOOOO. Hacking is basically building something. It could be anything.'
        },
        {
          question: 'Do I need to have programming experience?',
          answer: 'Basics of programming is enough.'
        },
        {
          question: 'How much do I have to pay to attend? ',
          answer: 'It’s FREE. :'
        },
        {
          question: 'Is it a team event?',
          answer: ' Yes. So the whole point of forming teams and working on a project gives you the opportunity to work in a real life setting. I mean seriously, that’s how it works in the industry. You have to learn to work with people from different background, different skill set, etc. What better way than a hackathon to get used to it? Teams include a maximum of 5 people. Our hackathons have “Meet-and-Greet” events before the actual event where you get to talk to attendees and look for teammates.'
        },

      
        {
          question: 'Why should I attend the hackathon? ',
          answer:'Why not? It’s a win- win situation for you.  And here’s why: •  FREE FOOD •  FREE SWAG •  Awards •  Meet new people •  LEARN.' 
          
        },
        
        {
          question: 'What can I hack at the hackathon?',
          answer: 'You can build anything. A website, a web app, Android/iOS App, Chrome extension, whatever you want to on a specific theme that will be given on the hackathon day.'
        },
        
],
      lorem:
        "Lorem ipsum dolor sit amet, at aliquam vivendum vel, everti delicatissimi cu eos. Dico iuvaret debitis mel an, et cum zril menandri. Eum in consul legimus accusam. Ea dico abhorreant duo, quo illum minimum incorrupte no, nostro voluptaria sea eu. Suas eligendi ius at, at nemore equidem est. Sed in error hendrerit, in consul constituam cum."
              
    };
  },

  methods: {
    getImageUrl(img) {
      return require("../assets/images/" + img);
    }
  }
};
</script>
