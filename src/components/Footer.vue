<template>
    <footer>
        <p> {{ copyright }}</p>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            copyright: 'Copyright 2018 The Nerd Cave'
        }
    }
}
</script>

<style scoped>
footer {
    background: #222;
    padding: 6px;
}

p {
    color: #dd9323;
    text-align: center;
}
</style>

