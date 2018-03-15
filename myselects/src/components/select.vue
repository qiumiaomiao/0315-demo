<template>
	<div class="selects">
		<select v-model="select1" id="select1">
			<option value="" selected>请选择</option>
			<option v-for="item in options" :value="item" v-bind:disabled="item == select2||item == select3">{{item}}</option>
		</select>
		<select v-model="select2" id="select2">
			<option value="" selected>请选择</option>
			<option v-for="item in options" :value="item" v-bind:disabled="item == select1||item == select3">{{item}}</option>
		</select>
		<select v-model="select3" id="select3">
			<option value="" selected>请选择</option>
			<option v-for="item in options" :value="item" v-bind:disabled="item == select2||item == select1">{{item}}</option>
		</select>
	</div>
</template>

<script>
	export default{
		data: function(){
			return{
				options:[1,2,3,4,5,6,7,8,9,10],
				select1:"",
				select2:"",
				select3:""
			}
		}
	}
</script>