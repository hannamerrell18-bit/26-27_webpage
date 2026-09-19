<template>
    <v-container>
        <v-row>
            <v-col :cols="12">
                <v-card>
                    <v-card-title>
                        <span class="text-h4 text--primary mt-0">2026-2027 Project Timeline</span>
                    </v-card-title>
                    <v-card-text>
                        <p class="timeline-section-title">Engineering Teams Timeline 2026-2027</p>
                            <p>Full-Year Master Timeline</p>
                            <img 
                                :src="require('@/assets/AY26/Timelines/master_timeline.png')" 
                                alt="RamBOTs 2026-2027 Full-Year Project Timeline" 
                                class="timeline-image"
                                @click="lightboxVisible = true"
                            >
                            <VueEasyLightbox
                            :visible="lightboxVisible"
                            :imgs="[require('@/assets/AY26/Timelines/master_timeline.png')]"
                            @hide="lightboxVisible = false"
                            />
                        <p class="timeline-hint">Click the timeline to enlarge </p>
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
import VueEasyLightbox from 'vue-easy-lightbox'

export default {
    components: {
        VueEasyLightbox,
    },
    data() {
        return {
            lightboxVisible: false,
        }
    },
}
</script>

<style scoped>
.timeline-section-title {
    text-decoration: underline;
    font-size: 1.3rem;
    font-weight: 400;
    margin-top: 1rem;
    color: #1E4D2B;
    text-align: left;
    margin-bottom: 10px;
}
.timeline-description{
    margin-bottom: 1rem;
}
.timeline-image {
    width: 100%;
    height: auto;
    cursor: pointer;
}
.timeline-hint {
    text-align: center;
    font-size: 0.9rem;
    font-style: italic;
    margin-botom:0.5rem;
}
</style>
