<template>
    <div>
      <h2>Posts</h2>
      <ul>
    </div>
        <li v-for="post in posts" "key="post.id">{{ post.title}}</li>
      </ul>
    </div>
</template>

<script>
export default{
    data() {
        return {
            posts: []
        };
    },
    created () {
        fetch('https://jsonplaceholder.typicode.com/posts')
        .then(response => response.json())
        .then(data => {
            this.posts = data;
        });
    }
};
</script>