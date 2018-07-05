<template>
    <div class="wrapper-d">
        <h4>我是组件D</h4>
        <div>A->D : {{val}}</div>
        <component-e :val="val"></component-e>
    </div>
</template>

<script>
import componentE from './componentE'
export default {
    components: {
        componentE
    },
    props: ['val']
}
</script>

<style>
    .wrapper-d {
        border: 1px solid lime;
    }
</style>


