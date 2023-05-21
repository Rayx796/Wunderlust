<script>
    import AboutImage from "../assets/images/about-banner.png"
</script>

<main>
    <!-- 
        - #ABOUT
      -->

      <section class="section about" id="about" aria-label="about">
        <div class="container">

          <figure class="about-banner">
            <img src={AboutImage} width="802" height="654" loading="lazy" alt="about banner"
              class="w-100">
          </figure>

          <div class="about-content">

            <h2 class="h2-sm section-title">We help you accomodate in germany, for your success future.</h2>

            <p class="section-text">
              Lorem Ipsum is simply dumm of free available in market the way printing and typesetting industry has been
              the industrys
              standard dummy text ever.
            </p>

            <ul class="about-list">

              <li class="has-before">
                Who are we 1
              </li>

              <li class="has-before">
                Who are we 1
              </li>

              <li class="has-before">
                Who are we 1
              </li>

            </ul>

            <div class="btn-group">
              <a href="#Why" class="btn btn-primary">Know More</a>

              <button class="flex-btn">
                <div class="btn-icon">
                  <ion-icon name="medal-outline" aria-hidden="true"></ion-icon>
                </div>

                <span class="span" id="Why"></span>
              </button>
            </div>

          </div>

        </div>
      </section>
</main>

<style>
  /*-----------------------------------*\
  #ABOUT
\*-----------------------------------*/

  .about .container {
    display: grid;
    gap: 30px;
  }

  .about-banner { filter: drop-shadow(2px 2px 5px hsla(0, 0%, 0%, 0.08)); }

  .about .section-text { margin-block: 20px 13px; }

  .about-list { margin-block-end: 50px; }

  .about-list .has-before {
    font-family: var(--ff-cuprum);
    font-size: var(--fs-8);
    font-weight: var(--fw-600);
    padding-inline-start: 20px;
    line-height: 1.5;
  }

  .about-list .has-before:not(:last-child) { margin-block-end: 15px; }

  .about-list .has-before::before {
    top: 10px;
    left: 0;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background-color: var(--go-red);
  }

  .about .btn-group { justify-content: flex-start; }

  .about .btn-group .flex-btn { gap: 10px; }

  .about .btn-icon ion-icon {
    color: var(--go-red);
    font-size: 40px;
  }

  .about .btn-group .span {
    color: var(--go-red);
    font-family: var(--ff-cuprum);
    font-size: var(--fs-6);
    font-weight: var(--fw-600);
  }
</style>