<template>
    <v-toolbar fixed class="blue">
        <v-toolbar-title class="mr-4">
            <span
                class="home"
                @click="navigateTo({name: 'register'})">
                TabTracker
            </span> 
        </v-toolbar-title>
        <!-- <v-toolbar-items>
            <v-btn flat dark>
                Browse
            </v-btn>
        </v-toolbar-items> -->

        <v-spacer></v-spacer>

        <v-toolbar-items>
            <v-btn flat dark
                @click="navigateTo({name: 'register'})">
                Sign Up
            </v-btn>
        </v-toolbar-items>
    </v-toolbar>
</template>

<script>
export default {
    methods: {
        navigateTo (route) {
            this.$route.push(route)
        }
    }
}
</script>

<style scoped>
.home {
    cursor: pointer;
}

.home:hover {
    color: #e9e;
}
</style>
