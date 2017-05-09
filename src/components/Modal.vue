<style lang="less">
  .vertical-center-modal{
    display: flex;
    align-items: center;
    justify-content: center;

    .ivu-modal{
      top: 0;
    }
  }
</style>
<template>
  <Button @click="modal9 = true">距离顶部 20px</Button>
  <Modal
    title="对话框标题"
    v-model="modal9"
    :styles="{top: '20px'}">
    <p>对话框内容</p>
    <p>对话框内容</p>
    <p>对话框内容</p>
  </Modal>
  <Button @click="modal10 = true">垂直居中</Button>
  <Modal
    title="对话框标题"
    v-model="modal10"
    class-name="vertical-center-modal">
    <p>对话框内容</p>
    <p>对话框内容</p>
    <p>对话框内容</p>
  </Modal>
</template>
<script>
  export default {
    data () {
      return {
        modal9: false,
        modal10: false
      }
    }
  }
</script>
