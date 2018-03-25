<template>
	<footer>
		<hr>
		<div class="container">
			&copy;<span v-once>{{ siteName }}</span> <span v-once>{{ currentYear }},
			developed by <a href="http://github.com/anindya-dhruba" target="_blank">tejal</a></span>
		</div>
	</footer>
</template>

<script>
	import {siteName} from '../../config';

	export default {
		created() {  console.log('/js/components/shared/appfooter.vue-- created');  },
	
		data() {
			return {
				siteName: siteName,
				currentYear: (new Date).getFullYear()
			}
		}
	}
</script>
