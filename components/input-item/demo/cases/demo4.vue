<template>
  <div class="md-example-child md-example-child-input-item-4">
    <md-field>
   

      <md-input-item
        ref="input11"
        title="自定义键盘"
        placeholder="custom number keyboard"
        is-virtual-keyboard
        virtual-keyboard-vm="myNumberKeyBoard"
        clearable
      ></md-input-item>
      <md-number-keyboard type="simple" ref="myNumberKeyBoard"></md-number-keyboard>
      
    </md-field>
  </div>
</template>

<script>
import {InputItem, NumberKeyboard, Field, Icon, Toast} from 'mand-mobile'
import '@examples/assets/images/bank-zs.svg'

export default {
  name: 'input-item-demo',
  /* DELETE */
  title: '表单控件',
  titleEnUS: 'Input with controls',
  message: '请在移动设备中扫码预览',
  messageEnUS: 'Please scan QR code and preview on mobile device',
  /* DELETE */
  components: {
    [InputItem.name]: InputItem,
    [NumberKeyboard.name]: NumberKeyboard,
    [Field.name]: Field,
    [Icon.name]: Icon,
  },
  methods: {
   
  },
}

</script>

<style lang="stylus">
.md-example-child-input-item-2
  .md-number-keyboard .md-popup-box
    max-width 720px
</style>
