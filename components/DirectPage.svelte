<script lang="ts">
  export let img: String, title: String, id: String, no: String;
</script>

<section {id} class="scroll-area">
  <div id="wrapper">
    <h3>Chapter {no}</h3>
    <h1>{title}</h1>
    <slot />
    <button>바로가기 ></button>
  </div>
  <img src={img} alt="" />
</section>

<style>
  * {
    margin: 0px;
    padding: 0px;
    scroll-behavior: smooth;
    color: white;
  }
  img {
    width: 100%;
    height: 100dvh;

    object-fit: cover;
    position: absolute;
    z-index: -1;
    background: gray;
    margin: 0px;
  }
  section {
    scroll-snap-align: start;
    height: 100dvh;

    font-family: "SUIT", sans-serif;
    display: flex;
    align-items: end;
  }

  h1 {
    font-size: 2.3em;
    font-weight: 900;
  }

  h2 {
    font-weight: 300;
    font-size: 1.6em;
    width: 80%;
  }

  h3 {
    font-weight: 300;
    color: #3a4ca8;
  }

  h1,
  h2,
  h3 {
    margin: 0px;
  }

  #wrapper {
    margin: 30px;
  }

  button {
    all: unset;
    border: 3px solid white;
    width: 180px;
    height: 40px;
    text-align: left;
    padding-left: 15px;
    margin-top: 10px;
    font-size: 18px;
    font-weight: 600;
    color: white;
    backdrop-filter: blur(5px);
    background: #ffffff38;
    cursor: pointer;
  }
</style>
