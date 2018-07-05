<template>
    <div class="wrapper-c">
        <h5>我是组件C</h5>
        <input type="text" v-model="val" @input="tell">
    </div>
</template>

<script>
export default {
    data(){
        return {
            val: ''
        }
    },
    methods: {
        tell() {
            setTimeout(() => {
                this.$emit('tellyou', this.val)
            }, 500);
        }
    }
}
</script>

<style>
    .wrapper-c{
        border: 1px solid red;
    }
</style>

