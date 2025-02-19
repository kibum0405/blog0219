<template>
    <div>
        <String label="이름" v-model="value.name" :editMode="editMode"/>
        <PostId offline label="postId" v-model="value.postId" :editMode="editMode" @change="change"/>

        <v-divider class="border-opacity-100 my-divider"></v-divider>
        <v-layout row justify-end>
            <v-btn
                width="64px"
                color="primary"
                @click="save"
            >
                저장
            </v-btn>
        </v-layout>
    </div>
</template>


<script>

import BaseEntity from './base-ui/BaseEntity.vue'

export default {
    name: 'Blog',
    mixins:[BaseEntity],
    components:{
    },
    
    data: () => ({
        path: "blogs"
    }),
    created(){
    },
    computed:{
    },
    methods: {
    },
}
</script>
