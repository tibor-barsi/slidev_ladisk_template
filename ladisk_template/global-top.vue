<template>
  <header class="absolute top-0 left-0 right-0 p-2 flex justify-between items-center bg-white/50">
    <div class="header-left">
      <!-- Add more logos here if needed -->
    </div>
    <div class="header-center">
      <img src="/UL_FS-ladisk_ENG-HOR-CMYK_color.png" alt="FS" class="logo" />
    </div>
    <div class="header-right">
      <!-- Add more logos here if needed -->
    </div>
  </header>
</template>

<style scoped>
header {
  height: 60px;
  z-index: 10;
}

.header-left,
.header-center,
.header-right {
  flex: 1;
  display: flex;
  align-items: center;
}

.header-left {
  justify-content: flex-start;
}

.header-center {
  height: 100px;
  width: auto;
  max-width: 800px;
  justify-content: center;
}

.header-right {
  justify-content: flex-end;
}

.logo {
  height: 70px;
  object-fit: contain;
}
</style>