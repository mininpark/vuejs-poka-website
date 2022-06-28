<template>
  <div v-on:mousemove="onCursor" id="cursor"></div>
</template>

<script>


export default {
  name: 'CursorCircle',
  method: {
    onCursor() {
    const cursor = document.getElementById('cursor');
    console.log(cursor)
    document.addEventListener('mousemove', (e) => {
    cursor.style.left = e.pageX + 'px';
    cursor.style.top = e.pageY + 'px';
    })
  }}
}
</script>

<style>
  #cursor {
    position: fixed;
    width:20px;
    height: 20px;
    border-radius: 50%;
    background: #fff;
    transition: 0.1s;
    transform: translate (-50%, -50%);
    pointer-events: none;
    mix-blend-mode: difference;
  }
</style>
