<template>
	<div class="weui-progress">
		<div class="weui-progress__bar">
			<div class="weui-progress__inner-bar js_progress" :style="{width: percent + '%'}"></div>
		</div>
		<a v-if="showClear" href="javascript:;" class="weui-progress__opr">
			<i class="weui-icon-cancel"></i>
		</a>
	</div>
</template>

<script>
import 'weui/dist/style/weui.min.css'

export default {
  name: 'vui-circle',

  props: {
    percent: Number,
    showClear: {
      type: Boolean,
      default: true
    }
  }
}
</script>