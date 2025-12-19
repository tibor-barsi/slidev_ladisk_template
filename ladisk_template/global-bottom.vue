<template>
  <footer class="absolute bottom-0 left-0 right-0 p-2 flex justify-between items-center bg-white/50">
    <span class="footer-left"></span>
    <span class="footer-center whitespace-nowrap">Footer 2025 - Ladisk</span>
    <span class="slidev-page-number">
      {{ $slidev.nav.currentPage }} / {{ $slidev.nav.total }}
    </span>
  </footer>
</template>

<style scoped>
footer {
  font-size: 0.8em;
  opacity: 0.7;
  z-index: 20;
}

.footer-left,
.footer-center,
.slidev-page-number {
  flex: 1;
}

.footer-left {
  text-align: left;
}

.footer-center {
  text-align: center;
}

.slidev-page-number {
  text-align: right;
}
</style>