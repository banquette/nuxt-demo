<script lang="ts">
import { Component } from "@banquette/vue-typescript";
import TodoComponent from "./todo/todo.component.vue";
import './main.css';

/**
 * The default theme defines the --bt-* variables used by the components
 * as well as some variants.
 */
import '@banquette/vue-ui/themes/default';

@Component({
    components: [TodoComponent]
})
export default class App {

}
</script>

<template>
    <div class="container">
        <h1>What do you want to do today?</h1>
        <todo></todo>
    </div>
</template>

<style>
.container {
    max-width: 750px;
    margin: 2rem auto;
    padding: 0 2rem;
}
</style>
