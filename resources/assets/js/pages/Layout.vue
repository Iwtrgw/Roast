<style type="text/css">
	
</style>

<template>
	<div id="app-layout">
		<navigation></navigation>
		<router-view></router-view>
	</div>
</template>

<script type="text/javascript">
	import Navigation from '../components/global/Navigation.vue';

	export default {
		components:{
			Navigation
		},
		creared(){
			this.$store.dispatch('loadCafes');
			this.$store.dispatch('loadUser');
		}
	}
</script>