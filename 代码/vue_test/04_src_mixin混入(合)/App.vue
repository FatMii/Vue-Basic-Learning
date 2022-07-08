<template>
	<div>
		<School/>
		<hr>
		<Student/>

1、对于data,methods,computed定义属性，组件中定义属性覆盖mixins中同名字段


2、对于created、mounted等生命周期函数，mixins中生命周期函数优先执行（执行顺序按mixins中顺序），再执行组件中生命周期函数


3.而对于相同的watch监听，mixins中的watch监听先执行。

	</div>
</template>

<script>
	import School from './components/School'
	import Student from './components/Student'

	export default {
		name:'App',
		components:{School,Student}
	}
</script>
