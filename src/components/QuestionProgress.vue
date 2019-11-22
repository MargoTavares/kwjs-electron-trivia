<template>
    <div class="progress-bar">
        <div>Score Progress: </div>
    </div>
</template>

<script lang="ts">
import {Component, Watch, Prop, Vue} from "vue-property-decorator";
import {ITrivia} from "@/types";

@Component
export default class QuestionProgress extends Vue {

}
</script>


<style lang="scss" scoped>
    .progress-bar {
        background-color: orange;
        max-width: 30rem;
        border-radius: 0.75rem;
        display: flex;
        flex-direction: column;
        padding: 1rem;
    }
</style>
