<template>
  <p class="greeting">
    <span class="one">&nbsp; Welcome!&nbsp; </span>
    •
    <span class="two">&nbsp; Benvenuto!&nbsp; </span>
    •
    <span class="three">&nbsp; Добро пожаловать!&nbsp; </span>
    •
    <span class="four">&nbsp; Willkommen!&nbsp; </span>
    •
    <span class="five">&nbsp; 欢迎!&nbsp; </span>
  </p>
</template>

<style scoped>
.greeting {
  overflow: hidden;
  color: var(--bg4);
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  padding: 2rem 0.5rem;
  justify-content: space-between;
}

@media only screen and (min-width: 400px) {
  .greeting {
    padding: 2rem 4rem;
  }
}

.one {
  color: var(--orange-dim);
}

.two {
  color: var(--green-dim);
}

.three {
  color: var(--yellow-dim);
}

.four {
  color: var(--blue-dim);
}

.five {
  color: var(--purple-dim);
}

.six {
  color: var(--aqua-dim)
}
</style>