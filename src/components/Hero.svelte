
<script>
  import HeroImage from "../assets/images/flag.png";
  import IoIosPlay from 'svelte-icons/io/IoIosPlay.svelte'

</script>
<main>
    <!-- 
        - #HERO
      -->

      <section class="section hero" id="home" aria-label="hero">
        <div class="container">

          <div class="hero-content">

            <p class="hero-subtitle has-before">Wellcome to Our Agency</p>

            <h1 class="h1 hero-title">Your Arrival To Germany Made Easy</h1>

            <p class="hero-text">
              Donec tincidunt lacinia diam, eu volutpat est sollicitudin at. Vestibulum ut mi tristi que, vulputate ante
              quis, tempus
              enim. Proin quis euismod purus. Suspen disse efficitur
              aliquam enim sed consequat vulputate ante quis.
            </p>

            <div class="btn-group">
              <a class="flex-btn" href="#about">
                <div class="btn-icon">
                  <div class="icon">
                    <IoIosPlay/>
                  </div>
                </div>
              </a>
              <h3  class="discover">Discover More </h3>
            </div>

          </div>

          <figure class="hero-banner has-before img-holder " style="--width: 650; --height: 650;">
            <img src={HeroImage} width="650" height="650" alt="hero banner" class="img-cover">
          </figure>

        </div>
      </section>
</main>

<style>

/*-----------------------------------*\
  #HERO
\*-----------------------------------*/
.icon {
    width: 30px;
    height: 30px;
  }

  .discover{
    color: var(--go-red);
  }

.hero {
    background-color: var(--red-bg);
    padding-block-start: calc(var(--section-padding) + 50px);
    text-align: center;
    overflow: hidden;
  }

  .hero .container {
    display: grid;
    gap: 50px;
  }

  .hero-subtitle {
    color: var(--go-red);
    font-size: var(--fs-12);
    font-weight: var(--fw-500);
    max-width: max-content;
    margin-inline: auto;
    z-index: 0;
  }

  .hero-subtitle::before {
    top: 8px;
    left: -20px;
    width: 15px;
    height: 2px;
    background-color: var(--go-red);
  }

  .hero-title { margin-block: 10px 15px; }

  .hero-text { color: var(--rich-black-fogra-29-1); }

  .hero .btn-group { margin-block-start: 40px; }

  .hero .btn-icon {
    background-color: var(--go-yellow);
    color: var(--white);
    font-size: 20px;
    padding: 20px;
    border-radius: 50%;
    animation: pulse 2s ease infinite;
  }

  @keyframes pulse {
    0% { box-shadow: 0 0 0 0 var(--go-yellow); }
    100% { box-shadow: 0 0 0 20px transparent; }
  }

  .hero .flex-btn .span {
    color: var(--go-red);
    font-size: var(--fs-9);
    font-weight: var(--fw-600);
  }

  .hero-banner,
  .hero-banner > img { border-radius: 50%; border: 4px solid var(--rich-black-fogra-29-2); }


</style>