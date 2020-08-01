<template>
  <div class="button">
    <p>{{type}}</p>
    <button :style="{ backgroundColor: color }">{{buttonText}}</button>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props: {
    type: String,
    buttonText: {
      type: String,
      default: 'Default'
    },
    color: String
  },
  data: function() {
    return {
      // styleObject: {
      //   fontSize: '13px',
      //   position: 'absolute',
      //   width: '81px',
      //   height: '36px',
      //   left: '319px',
      //   top: '141px',
      //   background: '#E0E0E0',
      //   boxShadow: '0px 2px 3px rgba(51, 51, 51, 0.2)',
      //   borderRadius: '6px',
      // }
    }
  }
}
</script>

<style scoped>
  button {
    position: absolute;
    width: 81px;
    height: 36px;
    box-shadow: 0px 2px 3px rgba(51, 51, 51, 0.2);
    border-radius: 6px;


  }
</style>
