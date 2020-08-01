<template>
  <div id="app">
    <div>
      <Button
        type="<Button />"
        color="#E0E0E0"
        />
    </div>
    <div>
      <Button
        type="&:hover, &:focus"
        color="#AEAEAE"
        class="hoverOne"
        />
    </div>
    <div>
      <Button
        type="<Button variant=”outline” />"
        color="white"
        class="outlineOne"
        />
    </div>
    <div>
      <Button
        type="&:hover, &:focus"
        color="white"
        class="outlineOne"
        id="hover"
        />
    </div>
  </div>
</template>

<script>
import Button from './components/Button.vue'

export default {
  name: 'App',
  components: {
    Button
  }
}
</script>

<style>
  #app {
    display: flex;
    justify-content: space-evenly;
  }

  .hoverOne button:hover {
      border: 2px solid #3D5AFE;
  }

  .outlineOne button {
    color: #3D5AFE;
    border: 1px solid #3D5AFE;
    border-radius: 6px;
  }
  #hover button:hover {
    border-width: 2px;
  }
</style>
