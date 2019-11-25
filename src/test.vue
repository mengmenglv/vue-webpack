<template>
    <div>
        <span @click="changeMsg">{{msg}}</span>
        <div>{{message}}</div>
    </div>

</template>

<script>
    export default {
        props: {
            msg:"thisdsd"
        },
        data() {
           return {
               message:'this is vue'
           }
        },
        methods: {
            changeMsg(){
                this.$emit('change','ling')
            }
        }
    }
</script>