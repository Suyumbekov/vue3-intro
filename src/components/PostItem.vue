<template>
   <div class="post">
        <div>
            <div><strong>Name:</strong> {{post.title}}</div>
            <div><strong>Feature:</strong> {{post.body}}</div>
        </div>
              <div @click="deletPost" class="post__btns">
                <my-button
                    @click="$emit('remove',post)"
                >
                    Удалить
                </my-button>
              </div>           
        </div>   
</template>

<script>
export default {
    props: {
        post: {
            type: Object,
            required: true
        }
    },
    methods: {
        deletPost(event){

        }
    }
    
}
</script>

<style scoped>
.post{
    padding: 10px;
    margin-top: 15px;
    border: 2px solid teal;
    display:flex;
    align-items: center;
    justify-content: space-between;
}
</style>
