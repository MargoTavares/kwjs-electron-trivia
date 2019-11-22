<template>
    <div class="feedback-form">
        <div>Feedback Form</div>
        <div></div>
        <button class="submit-form-btn" />
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
    .feedback-form {
        background-color: pink;
        max-width: 30rem;
        border-radius: 0.75rem;
        display: flex;
        flex-direction: column;
        padding: 1rem;
        height: 10rem;
    }

    .submit-form-btn {
        box-shadow:inset 0px 1px 0px 0px #f7c5c0;
        background-color:#fc8d83;
        border-radius:6px;
        border:1px solid #e68fac;
        display:inline-block;
        cursor:pointer;
        color:#ffffff;
        font-family:Arial;
        font-size:15px;
        font-weight:bold;
        padding:6px 24px;
        text-decoration:none;
        text-shadow:0px 1px 0px #c76a63;
        height: 5rem;
    }

    .submit-form-btn:hover {
            background-color: #fad0cd;
    }

    .submit-form-btn:active {
        position:relative;
        top: 1px;
    }
</style>
