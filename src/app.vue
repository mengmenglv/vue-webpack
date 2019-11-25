<template>
    <div id="app">{{text}}
    <test :msg="msg" @change="changeMessage"></test>
    </div>
</template>

<script>
    import Test from './test.vue'
    export default {
        components:{Test},
        data() {
            return {
                text: 'vue索testss',
                msg:"vue"
            }
        },
        methods: {
            changeMessage(val) {
                console.log(val);
                this.msg = val;
            }
        }
    }
</script>