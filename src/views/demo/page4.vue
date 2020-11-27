<template>
    <div>
        <Input style="width: 200px" v-model="item"/>
        <div>
            <strong>Square:</strong>
            <span v-square="item"></span>
        </div>
        <div>
            <strong>Root:</strong>
            <span v-sqrt="item"></span>
        </div>
        <div>
            <strong>Sine:</strong>
            <span v-sin="item"></span>
        </div>
        <div>
            <strong>Cosine:</strong>
            <span v-cos="item"></span>
        </div>
        <div>
            <strong>Tangent:</strong>
            <span v-tan="item"></span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'page4',
        data: function () {
            return {
                item: ''
            }
        }
    }
</script>

<style scoped>

</style>
