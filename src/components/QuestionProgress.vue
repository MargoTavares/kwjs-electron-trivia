<template>
    <div class="trivia-question">
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
    .trivia-question {
        background-color: lightcyan;
        max-width: 30rem;
        border-radius: 0.75rem;
        display: flex;
        flex-direction: column;
        padding: 1rem;

        .question-prompt {
            font-size: 1.5rem;
            color: hsl(0, 0%, 21%);
            text-align: center;
        }
        .answers-container {
            margin-top: 2rem;
            .possible-answer {
                background-color: hsl(210, 80%, 46%);
                color: whitesmoke;
                min-width: 25rem;
                padding: 0.75rem;
                border-radius: 0.25rem;
                &:not(:first-child) {
                    margin-top: 0.5rem;
                }
                font-size: 1rem;

                &:hover {
                    cursor: pointer;
                    filter: brightness(120%);
                }

                &.correct {
                    background-color: forestgreen;
                }

                &.incorrect {
                    background-color: orangered;
                }
            }

            display: flex;
            flex-direction: column;
            align-items: center;
        }
    }
</style>
