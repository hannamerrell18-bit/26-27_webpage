<template>
    <v-container>
        <v-row>
            <v-col :cols="$vuetify.display.mobile ? 12 : 4">
                <v-card height="100%">
                    <div class="d-flex flex-column justify-center">
                        <img width="80%" class="mt-6 mx-auto" :src="require('@/assets/RamLogoText.png')" />

                        <v-btn href="https://www.instagram.com/eceoutreachcsu/"
                            append-icon="mdi-link" variant="text" size="large" class="mx-8" target="_blank">
                            An ECE Outreach Project

                            <template v-slot:append>
                                <v-icon color="black"></v-icon>
                            </template>
                        </v-btn>

                        <v-btn href="https://www.youtube.com/channel/UC3K_Uz-jJc2ynTyCAwXKSBg" append-icon="mdi-youtube"
                            variant="text" size="large" class="mx-8" target="_blank">
                            Visit us on Youtube

                            <template v-slot:append>
                                <v-icon color="red"></v-icon>
                            </template>
                        </v-btn>

                        <v-btn href="https://github.com/RAMBotsCSU" append-icon="mdi-github" variant="text" size="large"
                            class="mx-8" target="_blank">
                            Visit us on Github

                            <template v-slot:append>
                                <v-icon color="black"></v-icon>
                            </template>
                        </v-btn>
                    </div>
                </v-card>
            </v-col>
            <v-col :cols="$vuetify.display.mobile ? 12 : 8">
                <v-card>
                    <v-carousel :height="$vuetify.display.mobile ? 250 : 425" show-arrows="hover" cycle
                        hide-delimiter-background>
                        <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src" cover></v-carousel-item>
                    </v-carousel>
                </v-card>
            </v-col>
        </v-row>
        <v-row class="justify-center">
            <v-col :cols="$vuetify.display.mobile ? 12 : 8">
                <v-card class="mb-4">
                    <v-card-text>
                        <div class="text-h3 text--primary mt-0">About Us</div>
                        <p class="text-h4 mt-4 section-header">Project Summary</p>
                        <p>
                            RamBOTs is an interdisciplinary senior design and outreach project focused on the
                            development, maintenance, and improvement of a quadruped robotic platform for
                            Colorado State University's Electrical and Computer Engineering outreach program.
                            The 2026–2027 team is working on developing the next-generation RamBOT 
                            (currently known as RamBOT MkII), while continuing to maintain Sparky, the existing robot.  

                        </p>

                        <p class="mt-6">
                            The project combines mechanical, electrical, computer, and software engineering
                            to create a reliable and engaging robotic demonstration platform. The team also
                            supports outreach events where RamBOT is used to introduce students and the
                            community to robotics and engineering.
                        </p>

                        <div class="text-h5 text--primary mt-10">Year 1:</div>
                        <p class="mt-2">
                            The first RamBOT team began by exploring machine-learning-based object detection
                            and adopting James Bruton's openDog platform as the mechanical foundation for
                            the project. During development, the team transitioned from the openDog V2
                            concept toward the newer V3 design and completed fabrication of several major
                            3D-printed components.
                        </p>

                        <div class="text-h5 text--primary mt-10">Year 2:</div>
                        <p class="mt-2">
                            The second-year team continued fabrication and assembly of the robot, integrating
                            the mechanical, electrical, and software systems. By the end of the year, the
                            platform was capable of basic quadruped motion, including walking and other
                            demonstration movements such as push-ups.
                        </p>

                        <div class="text-h5 text--primary mt-10">Year 3:</div>
                        <p class="mt-2">
                            The third-year team focused on understanding the existing system and improving
                            overall reliability. Sparky was used at multiple outreach events, while the team
                            also developed new capabilities such as tennis-ball tracking and management
                            scripts intended to make operation more consistent.
                        </p>

                        <div class="text-h5 text--primary mt-10">Year 4:</div>
                        <p class="mt-2">
                            The fourth-year team addressed major software compatibility issues after the
                            previous graphical user interface became deprecated. The team migrated Sparky
                            to a new software framework and added several outreach-oriented features,
                            including updated appearance elements and programmable LEDs. Gesture-detection
                            functionality was also developed and tested for future integration.
                        </p>

                        <div class="text-h5 text--primary mt-10">Year 5:</div>
                        <p class="mt-2">
                            The fifth-year team continued improving Sparky's reliability and usability,
                            with work spanning mechanical repairs, electrical development, software
                            migration, and integration of previously developed features. Their efforts
                            further highlighted several limitations of the existing platform and provided
                            important lessons for future RamBOT development.
                        </p>

                        <div class="text-h5 text--primary mt-10">Year 6:</div>
                        <p class="mt-2">
                            For the 2026-2027 school year, the senior design team is maintaining Sparky 
                            for continued outreach use while beginning development of the next-generation RamBOT platform. This new design
                            will build on lessons learned from the original robot, with greater emphasis on
                            reliability, maintainability, system integration, and long-term use by future
                            student teams.
                        </p>

                        <p class="text-h4 mt-12 section-header">Goals</p>

                        <p>
                            The primary goal of the 2026–2027 RamBOT project is to develop a reliable,
                            maintainable, and professional quadruped robot for use in CSU engineering outreach.
                            The team will also maintain Sparky so the existing platform remains available for
                            demonstrations during development of the new robot.
                        </p>

                        <div class="text-h5 text--primary mt-10">Mechanical</div>
                        <p class="mt-2">- Develop a durable mechanical platform for RamBOT Mk II that can handle repeated demonstrations and outreach events.</p>
                        <p class="mt-2">- Refine the leg and drivetrain design to improve mobility, stability, and ease of repair.</p>
                        <p class="mt-2">- Design components with practical manufacturing, assembly, and maintenance in mind.</p>
                        <p class="mt-2">- Use iterative prototype testing methods to guide improvements before committing to the final Mk II design.</p>

                        <div class="text-h5 text--primary mt-10">Computer and Software</div>
                        <p class="mt-2">- Develop a dependable software and controls foundation for RamBOT Mk II.</p>
                        <p class="mt-2">- Bring motors, sensors, and other hardware together into a coordinated control system.</p>
                        <p class="mt-2">- Build software that supports responsive movement and interactive outreach features.</p>
                        <p class="mt-2">- Create a codebase that is organized, documented, and easier for future RamBOT teams to continue developing.</p>

                        <div class="text-h5 text--primary mt-10">Electrical</div>
                        <p class="mt-2">- Build a reliable power and electrical architecture for RamBOT Mk II.</p>
                        <p class="mt-2">- Improve wiring and power distribution so the robot is easier to troubleshoot and maintain.</p>
                        <p class="mt-2">- Select and integrate electrical hardware that supports the robot’s mobility, sensing, and outreach features.</p>
                        <p class="mt-2">- Keep Sparky’s electrical systems functional and well documented for continued demonstrations.</p>

                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    data() {
        return {
            items: [
                 
                {
                    src: require('@/assets/AY26/Gallery/Team photo_fa26_V1.jpg'),
                    
                }
                
            ],
        };
    },
};
</script>

<style scoped>
.section-header {
    color: #1E4D2B;
    text-align: center;
    margin-bottom: 10px;
}

.section-header::after {
    content: "";
    display: block;
    width: 70px;
    height: 3px;
    background-color: #1E4D2B;
    margin: 4px auto 0;
}
</style>
