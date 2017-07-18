<template>
	<div>
		<a href="./home.html">home</a>
		<vhead></vhead>
		<vabout></vabout>
		<vfoot></vfoot>
	</div>
</template>

<script>
import vhead from '../../components/common/Head'
import vfoot from '../../components/common/Foot'
import vabout from '../../components/about/About'
export default {
	components: {
      vhead,
      vfoot,
      vabout
    }
}
</script>

<style>

</style>
