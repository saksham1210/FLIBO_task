<template>
	<div>
		<button
		@click="increase"
		>
			<h1>Click to increse Count</h1>
		</button>
		<div v-show="count!==0 && count!==10">
			<h1>{{count}}</h1>
		</div>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				count:0
			}
		},
		methods:{
			increase(){
				if (this.count===10){
					this.count=0
				}
				this.count++
			}
		}
	}

</script>

<style>
	button{
		background-color:red;
		width:200px;
		height:200px;
		border-radius: 100px;
	}
</style>
