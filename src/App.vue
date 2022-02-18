<template lang="pug">
#control
	textarea( v-model="values" )#grades
	#inputs
		#current
		input( type="text" )#wanted
		button#calculate Calculate
#results
	h1 Possibilities:
	ul
		li Result 1
		li Result 2
		li Result 3
		li Result 4
</template>

<script lang="ts" setup>
</script>

<style lang="sass">
#app
	width: 60vw
	height: 60vh
	@include debug
	#control
		text-area
		@include debug
		#inputs
			#current
			input
			#calculate
	#results
		h1
		ul
			li

*
	margin: 0
	padding: 0
	box-sizing: border-box

html, body
	height: 100vh

@mixin debug()
	border: 1px solid red

body
	display: flex
	align-items: center
	justify-content: center

</style>
