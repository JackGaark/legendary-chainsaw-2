<script>
  import { onMount } from 'svelte';

  let divStyle = ``;

  let div2Style = ``;

  let aStyle = ``;

  let div3Style = ``;

  onMount(() => {
    if (window.innerWidth <= 991) {
      divStyle += 'max-width: 100%;';
      aStyle += 'font-size: 40px;';
      div3Style += 'max-width: 100%;';
    }
  });

</script>


<section class="main-container">
  <div class="image-wrapper">
    <a href="..." class="title">Welcome</a>
    <div class="description">
      Lorem ipsum dolor sit amet consectetur. Leo justo enim et in. Aliquam at feugiat tortor purus quis eu ultrices quis tincidunt. Tellus integer egestas lectus ac.
    </div>
  </div>
</section>


<style>
  .main-container {
    justify-content: center;
    align-items: center;
    align-self: stretch;
    display: flex;
    margin-right: 1px;
    padding-top: 40px;
    padding-right: 20px;
    padding-bottom: 40px;
    padding-left: 20px;
    flex-direction: column;
    background-color: #bde3ff;
  }

  .image-wrapper {
    align-items: flex-start;
    align-self: center;
    display: flex;
    width: 736px;
    max-width: 100%;
    margin-top: 107px;
    margin-bottom: 107px;
    flex-direction: column;
  }

  .title {
    color: #000;
    font-family: Inter, sans-serif;
    font-size: 48px;
    font-weight: 500;
    line-height: 150%;
    letter-spacing: -0.528px;
    align-self: start;
    width: 209px;
  }

  .description {
    flex: 1 0 0;
    color: #000;
    font-family: Inter, sans-serif;
    font-size: 36px;
    font-weight: 500;
    line-height: 150%;
    letter-spacing: -0.396px;
    align-self: start;
    margin-top: 18px;
  }
</style>