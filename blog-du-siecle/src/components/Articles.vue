<template>
<div>
    <h1>Hello Vue!</h1>
    <div v-for="article in articles" :key ="article.title">
        <Article :article='article' />
    </div>    
</div>
</template>
<script>
import Article from "./Article";
export default {
    name:"Articles",
    data:()=>{
        return {articles :Articles}  
    },
    components: {
        Article
    }
};
const Articles = [

    {
        title:"Pourquoi les devs detestent PHP", 
        author:"angelus", 
        body: 'Le corps de l\'article',
        comments: [
            {
                title: 'commentaire 1',
                body: 'coprs de comment 1'
            },
            {
                title: 'commentaire 2',
                body: 'coprs de comment 2'
            }
        ]
    },
    {
        title:"Pourquoi les devs aiment vue.js", 
        author:"alilevautour",
        body: 'Le corps de l\'article',
        comments: [
            {
                title: 'commentaire 1',
                body: 'coprs de comment 1'
            },
            {
                title: 'commentaire 2',
                body: 'coprs de comment 2'
            }
        ]
    },
    {
        title:"Pourquoi les devs aiment bien node.js ", 
        auteur:"david",      
        body: 'Le corps de l\'article',
        comments: [
            {
                title: 'commentaire 1',
                body: 'coprs de comment 1'
            },
            {
                title: 'commentaire 2',
                body: 'coprs de comment 2'
            }
        ]
    }

];
</script>
<style scoped>

</style>