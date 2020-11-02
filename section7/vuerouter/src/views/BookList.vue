<template>
	<div>
		<h1>本の一覧</h1>
		<ul>
			<li v-for="book in books" @click="showBookDetail(book.id)" :key="book.id">
				{{ book.title }}
			</li>
		</ul>
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
	},
	methods: {
		showBookDetail(id) {
			this.bookIndex = id - 1
			console.log(this.bookIndex)
		}
	}
}
</script>

<style>

</style>