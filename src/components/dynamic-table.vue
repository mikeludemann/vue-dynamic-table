<template lang="html">

	<section class="dynamic-table">
		<table id='contact'>
			<tbody id="contentData">
				<tr>
					<th v-for="(key, value) in Object.keys(this.datas[0])" :key="value">{{key}}</th>
				</tr>
				<tr v-for="data in datas" :key="id">
					<td>{{data.id}}</td>
					<td>{{data.name}}</td>
					<td>{{data.age}}</td>
					<td>{{data.email}}</td>
				</tr>
			</tbody>
		</table>
	</section>

</template>

<script lang="js">

	export default {
		name: 'DynamicTable',
		props: {
			datas: {
				type: Array
			}
		},
		mounted () {

		},
		data () {
			return {

			}
		},
		methods: {

		},
		computed: {

		}
}


</script>

<style scoped lang="scss">
.dynamic-table {

}

#contact {
	text-align: center;
	font-family: "Trebuchet MS", Arial, Helvetica, sans-serif;
	border-collapse: collapse;
	border: 3px solid #ddd;
	width: 100%;
}

#contact td, #contact th {
	border: 1px solid #ddd;
	padding: 8px;
}

#contact tr:nth-child(even){background-color: #f2f2f2;}

#contact tr:hover {background-color: #ddd;}

#contact th {
	padding-top: 12px;
	padding-bottom: 12px;
	text-align: center;
	background-color: #15d81b;
	color: white;
}
</style>
