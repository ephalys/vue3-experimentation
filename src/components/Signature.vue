<script setup></script>

<template>
  <svg
    width="151"
    height="54"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 143.56 50.77"
  >
    <path
      class="signature-base"
      d="M55.14.29S33.41,48,16.11,49.91C.62,51.67,19,13.18,23,5.14a4.86,4.86,0,0,1,4-2.76c3.88-.25,9.95,4.07,10.6,33a14.61,14.61,0,0,0,2.71,8.22C46.22,51.9,61.16,63.77,74.14.15c0,0-25,79.33,4.76,28.68,0,0,.09,0,.08,0-.49,2.65-4.75,27.41,10,7.37a.93.93,0,0,1,1.5,0c1.47,2,5.71,5.41,15.78-.08a.49.49,0,0,1,.69.22c.58,1.4,2.88,4.88,10.33-.39a.5.5,0,0,1,.76.22c.69,2.12,4.55,8,25.29-2.32"
      stroke="#000"
      stroke-width="2"
    />
    <path
      class="signature-line"
      d="M0,18.51s119.28-5.78,137.87-.75"
      stroke="#000"
      stroke-width="2"
    />
  </svg>
</template>


<style lang="scss">
.signature {
  &-base {
    stroke-dasharray: 760px;
    animation: write-base 3s ease forwards;
    will-change: stroke-dasharray;
  }
  &-line {
    stroke-dasharray: 760px;
    animation: write-line 3s ease forwards;
    will-change: stroke-dasharray;
  }
}
@keyframes write-base {
  0% {
    stroke-dashoffset: 760px;
  }
  80% {
    stroke-dashoffset: 0;
  }
}

@keyframes write-line {
  0%,
  30% {
    stroke-dashoffset: 760px;
  }
  100% {
    stroke-dashoffset: 0;
  }
}
</style>