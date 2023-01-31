<template>
	<div>
		<Post 
		v-for="(a, i) in postData"
		:key="i"
		:postData="postData[i]"/>
	</div>
</template>

<script>
import Post from './Post.vue'
export default {
	name: 'ContainerVue',
	components: {
		Post
	},
	props: {
		postData: Array
	}
}
</script>

<style>

</style>