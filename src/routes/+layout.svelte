<script>
    import "../styles.css"
    import logo from "$lib/images/logo.svg"
    import shoppingCart from "$lib/images/shoppingCart.svg"
    import Hero from "../lib/components/Hero.svelte";

</script>

<div class="header">
  <img src={logo} alt="ward logo"/>
  <nav class="nav">
    <ul class="nav__list">
      <li class="nav__list-item"><a href="/">About</a></li>
      <li class="nav__list-item"><a href="/">Philosophy</a></li>
      <li class="nav__list-item"><a href="/">FAQ</a></li>
      <li class="nav__list-item"><a href="/">Contact</a></li>
    </ul>
  </nav>
  <a class="header__link" href="/">
      <img src={shoppingCart} alt="Shopping cart">
</div>

<main>
    <slot />
</main>

<style>
  .header {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 16px 0px;
    height: 96px;
    position: relative;
    background-color: #BDE3FF;
}
/* .header__link {
  font-size: 40px;
  font-weight: bold;
} */
.nav {
  width: 1120px;
  display: inline-block;
  justify-self: flex-start;
}
.nav__list {
  width: 1120px;
  display: flex;
  flex-wrap: wrap;
  height: 36px;
  align-items: center;
  gap: 16px 32px;
  position: relative;
}

.nav__list-item {
  margin-inline-end: 36px;
  font-size: 20px;
}

</style>

  