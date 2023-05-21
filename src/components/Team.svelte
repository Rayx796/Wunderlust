<script>
    import Persona from "../assets/images/persona.png"
</script>
<section class="section team">
    <h1 class="title">Our team</h1>
    <div class="container"></div>
        <div class="">
            <div style="box-wrapper">
                <div class="box black">
                    <div class="image-wrapper">
                        <img class="img-fluid" src={Persona} alt="..." />
                    </div>
                    <div class="box-desc">
                        <h5>Natalia</h5>
                        <p>CEO</p>
                    </div>
                    <ul class="social">
                        <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                        <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                        <li><a href="#"><i class="fab fa-pinterest-p"></i></a></li>
                    </ul>
                </div>
            </div>
            <div style="box-wrapper">
                <div class="box red">
                    <div class="image-wrapper">
                        <img class="img-fluid" src={Persona} alt="..." />
                    </div>
                    <div class="box-desc">
                        <h5>Daniela</h5>
                        <p>CEO</p>
                    </div>
                    <ul class="social">
                        <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                        <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                        <li><a href="#"><i class="fab fa-pinterest-p"></i></a></li>
                    </ul>
                </div>
            </div>
            <div style="box-wrapper">
                <div class="box yellow">
                    <div class="image-wrapper">
                        <img class="img-fluid" src={Persona} alt="..." />
                    </div>
                    <div class="box-desc">
                        <h5>X</h5>
                        <p>CEO</p>
                    </div>
                    <ul class="social">
                        <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                        <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                        <li><a href="#"><i class="fab fa-pinterest-p"></i></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

<style>
    .section{
        display: flex;
        flex-direction: column;
        justify-content: space-between;

    }
    .title{
        font-size: var(--fs-1);
        line-height: 1.1;
        color: var(--rich-black-fogra-29-1);
        font-family: var(--ff-cuprum);
        width: full;
        align-self: center;
        margin-bottom: 4rem;
    }
    
    .container{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
    }
    .img-fluid{
        width: 100%;
        height: auto;
    }
    .box-wrapper{
        margin-top: auto;
        margin-bottom: auto;
    }
    .box {
	border-radius: 150px;
    width: 100%;
	background:#fff;
	position:relative;
	overflow: hidden;
	text-align:center;
    --tw-shadow: 0 1px 2px 0 rgb(0 0 0 / 0.05);
    --tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);
    box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
    padding: 1rem;
    }
    .box.black:before{
        position: absolute;
        content: '';
        left: 0px;
        top: 0px;
        width: 100%;
        height: 100%;
        box-shadow: inset 0 0 25px rgba(0,0,0,0.30);
        transition: all 0.3s ease;
        background-image: linear-gradient(to right, #181717 0%, #382f2f 100%);
    }
    .box.red:before{
        position: absolute;
        content: '';
        left: 0px;
        top: 0px;
        width: 100%;
        height: 100%;
        box-shadow: inset 0 0 25px rgba(0,0,0,0.30);
        transition: all 0.3s ease;
        background-image: linear-gradient(to right, #c12b2b 0%, #f25757 100%);
    }
    .box.yellow:before{
        position: absolute;
        content: '';
        left: 0px;
        top: 0px;
        width: 100%;
        height: 100%;
        box-shadow: inset 0 0 25px rgba(0,0,0,0.30);
        transition: all 0.3s ease;
        background-image: linear-gradient(to right, #c7ba29 0%, #f2d857 100%);
    }
    .box:hover:before {
        width: 0px;
    }
    .box:hover .image-wrapper {
        padding:0;
    }
    .box-desc{
        color: #fff;
    }
    .box:hover .box-desc {
        color:black;
    }
    .box:hover .social li a {
        background:#fff;
        background-image: none;
        color:#000;
    }
    .box.black:hover .social li a:hover {
        background:#1d1d1d;
        color:#fff;
    }
    .box.red:hover .social li a:hover {
        background:#c12b2b;
        color:#fff;
    }
    .box.yellow:hover .social li a:hover {
        background:#c7ba29;
        color:#fff;
    }
    .image-wrapper {
        position: relative;
        max-width: 210px;
        max-height: 210px;
        margin:0 auto;
        overflow: hidden;
        border-radius: 50%;
        transition: all 0.5s ease;
        box-shadow: inset 0px 0px 20px rgba(0,0,0,0.20);
        margin-bottom: 0.75rem;
    }
    .image-wrapper img {
        border-radius: 50%;
        transition: all 500ms ease;
    }
    .box-desc {
        position:relative;
    }
    ul.social {
        padding:0;
    }
    ul.social li {
        display:inline-block;
        list-style-type:none;
    }
    .box.black ul.social li a {
        position:relative;
        width: 36px;
        height: 36px;
        background-image: linear-gradient(to right, #c12b2b 0%, #f25757 100%);
        display:inline-block;
        line-height:36px;
        border-radius:50%;
        color:#fff;
        transition: all .5s ease;
    }
    .box.red ul.social li a {
        position:relative;
        width: 36px;
        height: 36px;
        background-image: linear-gradient(to right, #282323 0%, #4e4444 100%);
        display:inline-block;
        line-height:36px;
        border-radius:50%;
        color:#fff;
        transition: all .5s ease;
    }
    .box.yellow ul.social li a {
        position:relative;
        width: 36px;
        height: 36px;
        background-image: linear-gradient(to right, #282323 0%, #4e4444 100%);
        display:inline-block;
        line-height:36px;
        border-radius:50%;
        color:#fff;
        transition: all .5s ease;
    }
    @media (max-width: 768px) {
        .box.black{
            border-radius: 0%;
        }
        .box.red{
            border-radius: 0%;
        }
        .box.yellow{
            border-radius: 0%;
        }

    }
</style>