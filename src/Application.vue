<script setup>
</script>

<template>
   <div class="container">
      <main>
         a
      </main>
      <aside>
         b
      </aside>
      <footer>
         dc
      </footer>
   </div>
</template>

<style lang="scss">
:root {
	--darker-grey: hsl(30, 12%, 77%);
}

.container {
  display: grid;
  grid-template-areas: 'main aside' 'footer footer';
  grid-template-columns: 1fr 300px;
  grid-template-rows: 1fr 100px;
  height: 100%;

  main {
   grid-area: main;
  }
  aside {
   grid-area: aside;
   border-left: 1px solid var(--darker-grey);
  }
  footer {
   grid-area: footer; 
   border-top: 1px solid var(--darker-grey);
  }
}
</style>
