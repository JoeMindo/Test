<template>
    <div>
       <h1 v-html="$page.post.title"></h1>
       <div v-html="$page.post.body"></div>
    </div>
    
</template>

<page-query>
query ($id: ID!){
    post(id: $id) {
        title
        body
    }
}
</page-query>

<script>
export default {
    metaInfo(){
        return {
            title: this.$page.post.title,
        }
    }
}
</script>