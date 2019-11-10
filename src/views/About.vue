<template>
  <div id="app">
  	<input v-model="message" class="form-control">
  <span v-if="seen" v-bind:title="time">
    {{ message }}
  </span>
</div>
</template>

<script type="text/javascript">
	export default {
  		data(){
    		return{ 
    				message:'testing',
    				time:'You loaded this page on ' + new Date().toLocaleString(),
    				seen:true
    			}
    }
  }
  		
</script>
