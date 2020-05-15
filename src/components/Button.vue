<template>
	<div class="main">
		<button
		@click="increase"
		>
			Click to increse Count
		</button>
		<div v-show="count!==0 && count!==10"><h1>{{count}}</h1></div>
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
	.main{
		height: 100vh;
		width:100vw;
		vertical-align: center;
	}
	button{
		vertical-align: center;
		background-color:red;
		width:200px;
		height:200px;
		border-radius: 100px;
	}
</style>
