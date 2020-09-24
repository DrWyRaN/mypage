<template>
    <div class="profile-page sidebar-collapse">
        <nav class="navbar navbar-expand-lg fixed-top navbar-transparent bg-primary" color-on-scroll="400">
            <div class="container">
                <div class="navbar-translate"><a class="navbar-brand" href="#" rel="tooltip">Creative CV</a>
                    <button class="navbar-toggler navbar-toggler" type="button" data-toggle="collapse" data-target="#navigation"
                            aria-controls="navigation" aria-expanded="false" aria-label="Toggle navigation"><span
                            class="navbar-toggler-bar bar1"></span><span class="navbar-toggler-bar bar2"></span><span
                            class="navbar-toggler-bar bar3"></span></button>
                </div>
                <div class="collapse navbar-collapse justify-content-end" id="navigation">
                    <ul class="navbar-nav">
                        <li class="nav-item"><a class="nav-link smooth-scroll" href="#about">About</a></li>
                        <li class="nav-item"><a class="nav-link smooth-scroll" href="#skill">Skills</a></li>
                        <li class="nav-item"><a class="nav-link smooth-scroll" href="#portfolio">Portfolio</a></li>
                        <li class="nav-item"><a class="nav-link smooth-scroll" href="#experience">Experience</a></li>
                        <li class="nav-item"><a class="nav-link smooth-scroll" @click="value1 = true" type="primary">Contact</a></li>
                    </ul>
                </div>
            </div>
        </nav>
        <Drawer title="Welcome to my page" :closable="false" v-model="value1">
            <p>Hello, sa</p>
            <p>Last login time: 2020-09-10 08:00:00</p>
        </Drawer>
    </div>
</template>

<script>
export default {
    name: "app-header",
    data() {
        return {
            value1: false
        }
    },
    props: ['headTitles'],
    methods: {}
}
</script>
