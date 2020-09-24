<template>
    <div id="app">
        <app-header v-if="header_show" :head-titles="headerTitle">
        </app-header>
        <router-view/>
        <app-footer></app-footer>
    </div>
</template>

<script>
import AppHeader from "./components/header";
import AppFooter from "./components/footer";

export default {
    name: 'App',
    components: {AppFooter, AppHeader},
    data() {
        return {
            header_show: true,
            headerTitle: ""
        }
    },
    methods: {
        header: function (bool, title) {
            this.header_show = bool;
            this.headerTitle = title;
        }
    }
}
</script>
