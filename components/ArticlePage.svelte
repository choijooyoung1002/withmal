<script>
	export let title, article, no, image;
</script>



<style>
  * {
    margin: 0px;
    padding: 0px;
    scroll-behavior: smooth;
  }

  section {
    scroll-snap-align: start;
    height: 100vh;
    font-family: "SUIT", sans-serif;
    display: flex;
    align-items: end;
  }

  h1 {
    font-size: 2.3em;
    font-weight: 900;
  }

  h2 {
    font-weight: 500;
    font-size: 1.6em;
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
    border: 3px solid #000000bd;
    width: 180px;
    height: 40px;
    text-align: left;
    padding-left: 15px;
    margin-top: 10px;
    font-size: 18px;
    font-weight: 600;
    color: #000000cf;
    backdrop-filter: blur(5px);
    background: #ffffff38;
    cursor: pointer;
  }
</style>


<section id="{title}" style="background: url({image}) no-repeat center;  background-size: cover;background-attachment: fixed;">

  <div id="wrapper"> 
    <h3>Chapter {no}</h3>
    <h1>{title}</h1>
    <h2>{description}</h2>
    <button>바로가기 ></button>
  </div>

</section>
