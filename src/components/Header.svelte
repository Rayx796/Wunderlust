<script>
  import IoMdClose from 'svelte-icons/io/IoMdClose.svelte'
  import IoIosMenu from 'svelte-icons/io/IoIosMenu.svelte'

  let y ;
  let menuActive = false;

  const handleScroll = (y) =>{
    if(y > 100){
      return "active"
    }
    return ""
  }

  const Switcher = () => {
    menuActive = !menuActive; 
  }

</script>
<main>
  <!-- 
    - #HEADER
  -->
  <header class={`header ${handleScroll(y)}`} data-header>
    <div class="container">

      <a href="#" class="logo">Wunderlust</a>

      <nav class={`navbar ${menuActive ? "active": ""}`} data-navbar>

        <div class="wrapper">
          <a href="#" class="logo">Wunderlust</a>

          <button class="nav-close-btn icon" aria-label="close menu" data-nav-toggler on:click={Switcher}>
              <IoMdClose />
          </button>
        </div>

        <ul class="navbar-list">

          <li>
            <a href="#home" class="navbar-link" data-nav-link>Home</a>
          </li>

          <li>
            <a href="#about" class="navbar-link" data-nav-link>About</a>
          </li>

          <li>
            <a href="#Why" class="navbar-link" data-nav-link>Why us?</a>
          </li>

          <li>
            <a href="#services" class="navbar-link" data-nav-link>Services</a>
          </li>

          <li>
            <a href="#team" class="navbar-link" data-nav-link>Our Team</a>
          </li>

          <li>
            <a href="#faq" class="navbar-link" data-nav-link>FAQ</a>
          </li>



        </ul>

      </nav>

      <button class="nav-open-btn icon" aria-label="open menu" data-nav-toggler on:click={Switcher} >
          <IoIosMenu/>
      </button>

      
      <a href="https://calendly.com/juanmiguelgarroni" class={`btn-outline ${handleScroll(y)}`}>Lets talk</a>
      <div class={`overlay ${menuActive ? "active": ""}`} on:click={Switcher} data-nav-toggler data-overlay></div>

    </div>
  </header>
</main>
<style>
      
  /*-----------------------------------*\
    #HEADER
  \*-----------------------------------*/

  .header .btn-outline { display: none; }

  .header {
    padding-block: 15px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 4;
  }

  .icon {
    width: 40px;
    height: 40px;
  }

  .header.active {
    background-color: var(--white);
    box-shadow: var(--shadow-2);
  }

  .header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    color: var(--rich-black-fogra-29-1);
    font-family: var(--ff-cuprum);
    font-size: 33px;
    font-weight: var(--fw-500);
    line-height: 1;
  }

  .nav-open-btn {
    color: var(--rich-black-fogra-29-1);
    font-size: 35px;
  }

  .navbar {
    position: fixed;
    top: 0;
    left: -280px;
    max-width: 280px;
    width: 100%;
    height: 100%;
    background-color: var(--rich-black-fogra-39);
    color: var(--white);
    padding: 30px 20px;
    visibility: hidden;
    transition: 0.25s var(--cubic-out);
    z-index: 4;
  }

  .navbar.active {
    visibility: visible;
    transform: translateX(280px);
    transition-duration: 0.5s;
  }

  .navbar .logo,
  .nav-close-btn { color: var(--white); }

  .navbar .wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-block-end: 25px;
  }

  .nav-close-btn { font-size: 30px; }

  .navbar-link {
    padding-block: 10px;
    transition: var(--transition-1);
  }

  .navbar-link:is(:hover, :focus) { color: var(--go-red); }

  .overlay {
    position: fixed;
    inset: 0;
    background-color: hsla(0, 0%, 100%, 0.7);
    visibility: hidden;
    opacity: 0;
    transition: var(--transition-1);
    z-index: 3;
  }

  .overlay.active {
    visibility: visible;
    opacity: 1;
  }

  @media (min-width: 575px) {
    .container {
    max-width: 540px;
    width: 100%;
    margin-inline: auto;
    }
    .header .container { max-width: unset; }
  }


  @media (min-width: 992px){
      /**
    * HEADER
    */

    .nav-open-btn,
    .navbar .wrapper,
    .overlay { display: none; }

    .header { padding: 20px; }

    .navbar,
    .navbar.active { all: unset; }

    .navbar-list {
      display: flex;
      gap: 40px;
    }

    .navbar-link {
      color: var(--rich-black-fogra-29-1);
      font-weight: var(--fw-500);
      padding-block: 0;
    }

    .header .btn-outline {
      display: block;
      color: var(--go-red);
      font-weight: var(--fw-600);
      text-transform: uppercase;
      border: 1px solid var(--go-red);
      padding: 7px 18px;
      transition: var(--transition-1);
    }

    .header .btn-outline:is(:hover, :focus) {
      background-color: darkred;
      color: rgb(231, 231, 231);
    }

    .btn-outline.active{
      background-color: var(--go-red);
      color: var(--white);
    }
  }

</style>

<svelte:window bind:scrollY={y} />