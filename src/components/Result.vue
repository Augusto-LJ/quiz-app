<script setup>
    import { defineProps } from 'vue';

    const {quizQuestionLength, numberCorrectAnswers} = defineProps(["quizQuestionLength","numberCorrectAnswers"])
</script>

<template>
    <div class="results">
        <p>Your result...</p>
        <h1>
            {{ numberCorrectAnswers }}/{{ quizQuestionLength }}
        </h1>
    </div>
</template>

<style scoped>
    .results {
        text-align: center;
        padding: 100px 0px;
    }

    p {
        font-size: 25px;
    }

    h1 {
        font-size: 80px;
    }
</style>