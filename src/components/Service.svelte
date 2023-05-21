<script>
  import Service1 from "../assets/images/service-1.png"
  import Service2 from "../assets/images/service-2.png"
  import Service3 from "../assets/images/service-3.png"
  import Service4 from "../assets/images/service-4.png"
</script>
<main>
    <!-- 
        - #SERVICE
      -->

      <section class="section service" id="services" aria-label="service">
        <div class="container">

          <p class="section-subtitle text-center">-What We Offer-</p>

          <h2 class="h2 section-title text-center">How we can help you</h2>

          <p class="section-text text-center">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi similique ipsam dolorum explicabo voluptas, deserunt tempore earum blanditiis recusandae qui.
          </p>

          <ul class="grid-list">

            <li>
              <div class="service-card has-after">

                <figure class="card-icon">
                  <img src={Service1} width="140" height="140" loading="lazy" alt="App Development"
                    class="img">
                </figure>

                <div class="card-content">

                  <h3 class="h3 card-title">Service 1</h3>

                  <p class="card-text">
                    Lorem ipsum dolor sit amet, consectetur adi piscing semper turpis. Nullam eget luctlie gula and
                    adipiscing elit.
                  </p>

                </div>

              </div>
            </li>

            <li>
              <div class="service-card has-after">

                <figure class="card-icon">
                  <img src={Service2} width="140" height="140" loading="lazy" alt="App Development"
                    class="img">
                </figure>

                <div class="card-content">

                  <h3 class="h3 card-title">Service 2</h3>

                  <p class="card-text">
                    Lorem ipsum dolor sit amet, consectetur adi piscing semper turpis. Nullam eget luctlie gula and
                    adipiscing elit.
                  </p>

                </div>

              </div>
            </li>

            <li>
              <div class="service-card has-after">

                <figure class="card-icon">
                  <img src={Service3} width="140" height="140" loading="lazy" alt="App Development"
                    class="img">
                </figure>

                <div class="card-content">

                  <h3 class="h3 card-title">Service 3</h3>

                  <p class="card-text">
                    Lorem ipsum dolor sit amet, consectetur adi piscing semper turpis. Nullam eget luctlie gula and
                    adipiscing elit.
                  </p>

                </div>

              </div>
            </li>

            <li>
              <div class="service-card has-after">

                <figure class="card-icon">
                  <img src={Service4} width="140" height="140" loading="lazy" alt="App Development"
                    class="img">
                </figure>

                <div class="card-content">

                  <h3 class="h3 card-title">Service 4</h3>

                  <p class="card-text">
                    Lorem ipsum dolor sit amet, consectetur adi piscing semper turpis. Nullam eget luctlie gula and
                    adipiscing elit.
                  </p>

                </div>

              </div>
            </li>
          </ul>

          <a href="https://calendly.com/juanmiguelgarroni" class="btn btn-primary" id="team">Get Started</a>

        </div>
      </section>
</main>

<style>
  .service{background-color: rgb(249, 249, 249);}

  .service .section-text { margin-block: 15px 50px; }

  .service .grid-list { margin-block-end: 50px; }

  .service-card {
    height: 100%;
    padding: 30px 25px;
    text-align: center;
    box-shadow: var(--shadow-1);
  }

  .service-card::after {
    bottom: 0;
    left: 0;
    width: 0;
    height: 2px;
    background-color: var(--go-red);
    transition: var(--transition-2);
  }

  .service-card:is(:hover, :focus-within)::after { width: 100%; }

  .service-card .card-icon {
    max-width: max-content;
    margin-inline: auto;
    margin-block-end: 10px; 
  }

  .service-card .img { transition: var(--transition-1); }

  .service-card:is(:hover, :focus-within) .img { transform: scale(1.1); }

  .service-card .card-text { margin-block: 5px 13px; }

  .service .btn { margin-inline: auto; }

</style>