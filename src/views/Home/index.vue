<template lang="html">
    <div class="container">
        <h1>Welcome to Z-Vue{{ obj.name }}</h1>
        <img class="logo" src="https://note.ss.purevivi.chat/Fnn562fSUBw4HdUH7GOH8sWD0GnH" />
        <a href="#/page1">page1</a>
    </div>
</template>

<script lang="ts">
interface Obj {
    name: string
}
import { PropType } from 'vue'

export default {
    name: 'HelloHome',
    props: {
        msg: {
            type: String,
            default: ''
        },
        obj: {
            type: Object as PropType<Obj>,
            default: {}
        }
    }
}
</script>

<style lang="scss">
.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;
}

.logo {
    width: 100px;
    height: 100px;
    border-radius: 50%;
}

h1 {
    color: $blue;
}
</style>
