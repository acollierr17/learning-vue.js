<template>
    <div id="nerds">
        <ul>
            <li v-for="nerd in nerds" :key="nerd" @click="nerd.show = !nerd.show">
                <h2>{{ nerd.name }}</h2>
                <h3 v-show="nerd.show">{{ nerd.speciality }}</h3>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data() {
        return {
            nerds: [
                {name: 'Hailey', speciality: 'Vue Components', show: false},
                {name: 'John', speciality: 'HTML Wizardry', show: false},
                {name: 'Thomas', speciality: 'Click Events', show: false},
                {name: 'Ellie', speciality: 'Conditionals', show: false},
                {name: 'Jessica', speciality: 'Webpack', show: false},
                {name: 'Dani', speciality: 'Data Diggin', show: false}
            ]
        }
    }
}
</script>

<style scoped>
#nerds {
    width: 100%;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
}
ul {
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
}
li {
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
}
</style>

