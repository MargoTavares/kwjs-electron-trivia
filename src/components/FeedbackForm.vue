<template>
    <div class="trivia-question">
        <div>Feedback Form</div>
        <button class="submit-form" />
    </div>
</template>

<script lang="ts">
import {Component, Watch, Prop, Vue} from "vue-property-decorator";
import {ITrivia} from "@/types";

@Component
export default class FeedbackForm extends Vue {

}
</script>


<style lang="scss" scoped>
    .trivia-question {
        background-color: lightcyan;
        max-width: 30rem;
        border-radius: 0.75rem;
        display: flex;
        flex-direction: column;
        padding: 1rem;
    }
</style>
