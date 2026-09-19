<template>
    <div>
        <div class="ece-logo-section">
            <img  
                :src="require('@/assets/Logos/ECE_CSU_logo.png')"
                alt="Colorado State University Electrical and Computer Engineering"
                class="ece-logo"
            >
        </div>
    </div>
    <v-footer bottom color="primary">
        <v-row justify="center" no-gutters>
            <v-col class="py-1 text-center text-white text-overline" cols="12">
                <a href="https://give.colostate.edu/campaigns/40250/donations/new"
                    class="text-white text-decoration-underline">Support our program</a>
                |
                <a href="https://www.engr.colostate.edu/ece/senior-design/"
                    class="text-white text-decoration-underline">Other ECE Sr. Design projects</a>
                |
                <a href="https://www.engr.colostate.edu/ece/" class="text-white text-decoration-underline">ECE
                    Department</a>
                |
                <a href="http://www.colostate.edu/" class="text-white text-decoration-underline">CSU main
                    website</a>
            </v-col>
        </v-row>
    </v-footer>
</template>

<script>
export default {
    data: () => ({}),
}
</script>

<style scoped>
.ece-logo-section {
    text-align: center;
    padding: 24px 16px;
}
.ece-logo {
    width: 100%;
    max-width: 600px;
    height: auto;
}
</style>