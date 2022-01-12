<template>
    <div>
        <h1>Hello World from page 2 </h1>
         <Card/>
    </div>
   
</template>
<script>
import Card from '../../components/Card.vue';

export default {
    name: 'Other Page',
    components: {
        Card
    }
}
</script>