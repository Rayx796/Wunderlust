<script>
  let cardActive1 = false;
  let cardActive2 = false;
  let cardActive3 = false;
  let cardActive4 = false;
  let cardActive5 = false;

  const Switcher1 = () => {cardActive1 = !cardActive1;}
  const Switcher2 = () => {cardActive2 = !cardActive2;}
  const Switcher3 = () => {cardActive3 = !cardActive3;}
  const Switcher4 = () => {cardActive4 = !cardActive4;}
  const Switcher5 = () => {cardActive5 = !cardActive5;}
    

</script>



<section class="section faq" aria-label="frequently asked questions" id="faq">
  <div class="container">

    <div class="title-wrapper">
      <h2 class="h2 section-title">Discover Frequently Asked Questions?</h2>

      <a href="https://calendly.com/juanmiguelgarroni" class="btn btn-primary">Lets Talk</a>
    </div>

    <ul class="grid-list">

      <li>
        <div class="faq-card">

          <button class={`card-action ${cardActive1 ? "active": ""}`} data-accordion-action on:click={Switcher1}>
            <h3 class="h3 card-title">
              01. Question 1?
            </h3>

            <div class="action-icon">
              <ion-icon name="add-outline" aria-hidden="true" class="open"></ion-icon>
              <ion-icon name="remove-outline" aria-hidden="true" class="close"></ion-icon>
            </div>
          </button>

          <div class="card-content">
            <p>
              Morbi aliquam quis quam in luctus. Nullam tincidunt pulvinar imperdiet. Sed varius, diam vitae
              posuere semper, libero ex
              hendrerit nunc, ac sagittis eros metus ut diam. Donec a nibh in libero maximus vehicula. Etiam sit
              amet condimentum
              erat. Pellentesque ultrices sagittis turpis, quis tempus ante viverra et.Morbi aliquam quis quam in
              luctus. Nullam
              tincidunt pulvinar imperdiet. Sed varius, diam vitae posuere semper, tincidunt pulvinar imperdiet.
              Sed varius, diam
              vitae posuere semper.
            </p>
          </div>

        </div>
      </li>

      <li>
        <div class="faq-card">

          <button class={`card-action ${cardActive2 ? "active": ""}`} data-accordion-action on:click={Switcher2}>
            <h3 class="h3 card-title">
              02. Question 2?
            </h3>

            <div class="action-icon">
              <ion-icon name="add-outline" aria-hidden="true" class="open"></ion-icon>
              <ion-icon name="remove-outline" aria-hidden="true" class="close"></ion-icon>
            </div>
          </button>

          <div class="card-content">
            <p>
              Morbi aliquam quis quam in luctus. Nullam tincidunt pulvinar imperdiet. Sed varius, diam vitae
              posuere semper, libero ex
              hendrerit nunc, ac sagittis eros metus ut diam. Donec a nibh in libero maximus vehicula. Etiam sit
              amet condimentum
              erat. Pellentesque ultrices sagittis turpis, quis tempus ante viverra et.Morbi aliquam quis quam in
              luctus. Nullam
              tincidunt pulvinar imperdiet. Sed varius, diam vitae posuere semper, tincidunt pulvinar imperdiet.
              Sed varius, diam
              vitae posuere semper.
            </p>
          </div>

        </div>
      </li>

      <li>
        <div class="faq-card">

          <button class={`card-action ${cardActive3 ? "active": ""}`} data-accordion-action on:click={Switcher3}>
            <h3 class="h3 card-title">
              03. Question 3?
            </h3>

            <div class="action-icon">
              <ion-icon name="add-outline" aria-hidden="true" class="open"></ion-icon>
              <ion-icon name="remove-outline" aria-hidden="true" class="close"></ion-icon>
            </div>
          </button>

          <div class="card-content">
            <p>
              Morbi aliquam quis quam in luctus. Nullam tincidunt pulvinar imperdiet. Sed varius, diam vitae
              posuere semper, libero ex
              hendrerit nunc, ac sagittis eros metus ut diam. Donec a nibh in libero maximus vehicula. Etiam sit
              amet condimentum
              erat. Pellentesque ultrices sagittis turpis, quis tempus ante viverra et.Morbi aliquam quis quam in
              luctus. Nullam
              tincidunt pulvinar imperdiet. Sed varius, diam vitae posuere semper, tincidunt pulvinar imperdiet.
              Sed varius, diam
              vitae posuere semper.
            </p>
          </div>

        </div>
      </li>

      <li>
        <div class="faq-card">

          <button class={`card-action ${cardActive4 ? "active": ""}`} data-accordion-action on:click={Switcher4}>
            <h3 class="h3 card-title">
              04. Question 4?
            </h3>

            <div class="action-icon">
              <ion-icon name="add-outline" aria-hidden="true" class="open"></ion-icon>
              <ion-icon name="remove-outline" aria-hidden="true" class="close"></ion-icon>
            </div>
          </button>

          <div class="card-content">
            <p>
              Morbi aliquam quis quam in luctus. Nullam tincidunt pulvinar imperdiet. Sed varius, diam vitae
              posuere semper, libero ex
              hendrerit nunc, ac sagittis eros metus ut diam. Donec a nibh in libero maximus vehicula. Etiam sit
              amet condimentum
              erat. Pellentesque ultrices sagittis turpis, quis tempus ante viverra et.Morbi aliquam quis quam in
              luctus. Nullam
              tincidunt pulvinar imperdiet. Sed varius, diam vitae posuere semper, tincidunt pulvinar imperdiet.
              Sed varius, diam
              vitae posuere semper.
            </p>
          </div>

        </div>
      </li>

      <li>
        <div class="faq-card">

          <button class={`card-action ${cardActive5 ? "active": ""}`} data-accordion-action on:click={Switcher5}>
            <h3 class="h3 card-title">
              05. Question 5?
            </h3>

            <div class="action-icon">
              <ion-icon name="add-outline" aria-hidden="true" class="open"></ion-icon>
              <ion-icon name="remove-outline" aria-hidden="true" class="close"></ion-icon>
            </div>
          </button>

          <div class="card-content">
            <p>
              Morbi aliquam quis quam in luctus. Nullam tincidunt pulvinar imperdiet. Sed varius, diam vitae
              posuere semper, libero ex
              hendrerit nunc, ac sagittis eros metus ut diam. Donec a nibh in libero maximus vehicula. Etiam sit
              amet condimentum
              erat. Pellentesque ultrices sagittis turpis, quis tempus ante viverra et.Morbi aliquam quis quam in
              luctus. Nullam
              tincidunt pulvinar imperdiet. Sed varius, diam vitae posuere semper, tincidunt pulvinar imperdiet.
              Sed varius, diam
              vitae posuere semper.
            </p>
          </div>

        </div>
      </li>
      

    </ul>

  </div>
</section>


<style>
   
/*-----------------------------------*\
  #FAQ
\*-----------------------------------*/

.faq .container {
  display: grid;
  gap: 20px;
}

.faq .title-wrapper {
  background-color: var(--white);
  padding: 30px 25px;
  box-shadow: var(--shadow-1);
}

.faq .section-title {
  font-size: var(--fs-4);
  margin-block-end: 30px;
}

.faq-card {
  background-color: var(--go-red_5);
  border-radius: var(--radius-5);
  overflow: hidden;
}

.faq-card .card-action {
  --action-bg: var(--go-red_8);
  --color: var(--granite-gray);

  background-color: var(--action-bg);
  text-align: left;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 25px;
  gap: 20px;
  transition: var(--transition-1);
}

.faq-card .card-action:is(:hover, :focus, .active) {
  --action-bg: var(--go-red);
  --color: var(--white);
}

.faq-card .card-title {
  color: var(--color);
  font-size: var(--fs-8);
  transition: var(--transition-1);
}

.faq-card ion-icon {
  color: var(--color);
  font-size: 15px;
  transition: var(--transition-1);
  --ionicon-stroke-width: 60px;
}

.faq-card .card-action.active .open,
.faq-card .card-action .close { display: none; }

.faq-card .card-action .open,
.faq-card .card-action.active .close { display: block; }

.faq-card .card-content {
  font-size: var(--fs-10);
  padding-inline: 25px;
  max-height: 0;
  overflow: hidden;
  transition: var(--transition-2);
}

.faq-card .card-content p { margin-block: 15px; }

.faq-card .card-action.active + .card-content { max-height: 500px; }

</style>

