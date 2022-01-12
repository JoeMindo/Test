<template>
<div class="card">
    {{message}}
    <button @click="onClick">
        Change
    </button>
</div>
</template>

<script>
export default {
    name: 'Card',
    data(){
        return {
            message: 'Hey there! Try changing me'
        }
    },
    methods: {
        onClick () {
            this.message = 'New message'
        }
    }
}
</script>
<style>
.card {
  padding: 20px;
  background: #FFF;
}
</style>