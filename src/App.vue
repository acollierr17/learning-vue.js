<template>
<div>
    <app-header :title="title" @changeTitle="updateTitle($event)"></app-header>
    <app-nerds :nerds="nerds"></app-nerds>
    <app-footer :title="title"></app-footer>
</div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Nerds from './components/Nerds.vue';

export default {
    components: {
        'app-header': Header,
        'app-footer': Footer,
        'app-nerds': Nerds
    },
    data() {
        return {
            nerds: [{
                    name: 'Hailey',
                    speciality: 'Vue Components',
                    show: false
                },
                {
                    name: 'John',
                    speciality: 'HTML Wizardry',
                    show: false
                },
                {
                    name: 'Thomas',
                    speciality: 'Click Events',
                    show: false
                },
                {
                    name: 'Ellie',
                    speciality: 'Conditionals',
                    show: false
                },
                {
                    name: 'Jessica',
                    speciality: 'Webpack',
                    show: false
                },
                {
                    name: 'Dani',
                    speciality: 'Data Diggin',
                    show: false
                }
            ],
            title: 'Vue Nerds'
        }
    },
    methods: {
      updateTitle: function(updatedTitle) {
        this.title = updatedTitle;
      }
    }
}
</script>

<style>

</style>
