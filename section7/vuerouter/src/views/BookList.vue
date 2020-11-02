<template>
	<div>
		bookList
	</div>
</template>

<script>
export default {
	name: 'BookList',
	data() {
		return {
			bookIndex: -1,
			books: [
				{id: 1, title: 'タイトル1', content: '内容1'},
				{id: 2, title: 'タイトル2', content: '内容2'},
				{id: 3, title: 'タイトル3', content: '内容3'},
			]
		}
	}
}
</script>

<style>

</style>