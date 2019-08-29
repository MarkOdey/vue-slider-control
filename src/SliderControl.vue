<template>
  <div>

      <div :class="{
          vertical : orientation == 'vertical',
          horizontal : orientation == 'horizontal'
      }" class="slider-container"></div>

      <div class="slider-value"></div>

  </div>
</template>

<script>
export default {
            props: {
            'value': {
                type: Number,
                required: true
            },
            'max': {
                type: Number,
                default: 100
            },
            'min': {
                type: Number,
                default: 0
            },
            'stepSize': {
                type: Number,
                default: 1
            },
            'disabled': {
                type: Boolean,
                default: false
            },
            'size': {
                type: Number,
                default: 100
            },
            'responsive': {
                type: Boolean,
                default: false
            },
            'orientation' : {
                type: String,
                default:"vertical"
            },
            'primaryColor': {
                type: String,
                default: '#409eff'
            },
            'secondaryColor': {
                type: String,
                default: '#dcdfe6'
            },
            'textColor': {
                type: String,
                default: '#000000'
            },
            'strokeWidth': {
                type: Number,
                default: 17
            },
            'valueDisplayFunction': {
                type: Function,
                default: (v) => v
            }
         
        },
        methods: {

        }

}
</script>

<style>

</style>