<script setup>
import { ref } from 'vue';
const x = ref(0);
const y = ref(0);
const result = ref(0);
</script>

<template>
	<div class="...">
		<input type="text" id="x" v-model="x" class="number">
		<button id="add" type="button" @click="result = parseInt(x) + parseInt(y)"> + </button>
		<button id="sub" type="button" @click="result = x-y"> - </button>
		<button id="mul" type="button" @click="result = x*y"> * </button>
		<button id="div" type="button" @click="result = x /y"> / </button>
		<input type="text" id="y" v-model="y" class="number"> =
		<input type="text" id="result" v-model="result" class="number">
	</div>
</template>

<style>
.number{
	padding:10px;
	width: 120px;
}
</style>