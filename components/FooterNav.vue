<template>
    <v-footer border>
        <v-row justify="center" no-gutters>
            <v-btn variant="text" class="mx-2" rounded="xl" href="/">
                Home
            </v-btn>
            <v-btn variant="text" class="mx-2" rounded="xl" href="/">
                About Us
            </v-btn>
            <v-btn variant="text" class="mx-2" rounded="xl" href="/">
                Team
            </v-btn>
            <v-col class="text-center mt-4" cols="12">
                {{ new Date().getFullYear() }} — <strong><a href="https://www.meeovi.com">The Meeovi Company</a></strong>
            </v-col>
        </v-row>
    </v-footer>
</template>

<script>
    export default {}
</script>