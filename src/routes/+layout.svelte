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

  <section class="features">
        <div class="wrapper">
            <ul>
                <li>
                    <strong>
                        <span>Secure</span>
                    </strong>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Bibendum eget suspendisse metus lacus vel massa suspendisse aliquam nisi.</p>
                </li>
                <li>
                    <strong>
                        <span>Fast</span>
                    </strong>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Bibendum eget suspendisse metus lacus vel massa suspendisse aliquam nisi.</p>
                </li>
                <li>
                    <strong>
                        <span>Reliable</span>
                    </strong>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Bibendum eget suspendisse metus lacus vel massa suspendisse aliquam nisi.</p>
                </li>
            </ul>
        </div>
    </section>

<main>
    <slot />
</main>

<style>
  .header {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 16px;
    height: 96px;
    position: relative;
    background-color: #BDE3FF;
}
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


.features {
  display: flex;
  width: auto;
  height: 600px;
  top: 0;
  left: 0;
  background-color: #d9d9d9;
}

.features .wrapper {
    transform: skewY(-12deg); /* UN-SKEW */
}
.features .wrapper ul {
    display: flex;
    flex-direction: column;
    gap: 3em;
    padding: 5em 0 10em;
}


</style>

  