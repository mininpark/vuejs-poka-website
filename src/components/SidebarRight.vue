<template>
  <div class="SidebarRight">
    <div class="SidebarRight__track">
      <a class="SidebarRight__track--content">&nbsp;for more information&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information&nbsp;Click for more information Click</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SidebarRight',
  
}
</script>

<style lang="scss">
.SidebarRight {
  transform: rotate(90deg);
  right: 0%;
  top: 5%;
  font-size: 1.5rem; 
  color: red;
  position: fixed;
  }
.SidebarRight .SidebarRight__track {
  position: absolute;
  white-space: nowrap;
  will-change: transform;
  animation: marquee-right 60s linear infinite; 
  animation-direction:reverse;
  }

@keyframes marquee-right {
  from { transform: translateX(-50%); }
  to { transform: translateX(0%); }
}

</style>