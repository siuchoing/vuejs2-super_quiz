<template>
    <div class="panel panel-default">
        <div class="panel-heading">
            <h3 class="panel-title text-center">{{ question }}</h3>
        </div>
        <div class="panel-body">
            <div class="col-xs-12 col-sm-6 text-center">
                <button
                        class="btn btn-primary btn-lg"
                        style="margin: 10px"
                        @click="onAnswer(btnData[0].correct)"
                >{{ btnData[0].answer }}</button>
            </div>
            <div class="col-xs-12 col-sm-6 text-center">
                <button
                        class="btn btn-primary btn-lg"
                        style="margin: 10px"
                        @click="onAnswer(btnData[1].correct)"
                >{{ btnData[1].answer }}</button>
            </div>
            <div class="col-xs-12 col-sm-6 text-center">
                <button
                        class="btn btn-primary btn-lg"
                        style="margin: 10px"
                        @click="onAnswer(btnData[2].correct)"
                >{{ btnData[2].answer }}</button>
            </div>
            <div class="col-xs-12 col-sm-6 text-center">
                <button
                        class="btn btn-primary btn-lg"
                        style="margin: 10px"
                        @click="onAnswer(btnData[3].correct)"
                >{{ btnData[3].answer }}</button>
            </div>
        </div>
    </div>
</template>
<style>

</style>
<script>
    export default{
        data() {
            return {
                question: 'This is a question',
                btnData: [
                    {correct: true, answer: 0},
                    {correct: false, answer: 0},
                    {correct: false, answer: 0},
                    {correct: false, answer: 0}
                ]
            };
        },
        methods: {
            onAnswer(isCorrect) {
            }
        }
    }
</script>
