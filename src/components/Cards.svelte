<script>
    import Data from "../assets/images/data.png"
    import Sketch from "../assets/images/sketch.png"
    import Startup from "../assets/images/startup.png"

</script>
<section class="section why" >
    <h2 class="title" >Why Us?</h2>
    <div class="container">
        <div class="card">
            <div class="imgBx">
                <img src={Sketch} alt="">
                <h3>Quality 1</h3>
            </div>
            <div class="content">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore dolorem minima nobis accusantium animi nihil, id quo deleniti officiis illum rem magni ea adipisci iure atque magnam expedita? Facilis, pariatur.</p>
            </div>
        </div>
        <div class="card">
            <div class="imgBx">
                <img src={Data}  alt="">
                <h3>Quality 2</h3>
            </div>
            <div class="content">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore dolorem minima nobis accusantium animi nihil, id quo deleniti officiis illum rem magni ea adipisci iure atque magnam expedita? Facilis, pariatur.</p>
            </div>
        </div>
        <div class="card">
            <div class="imgBx">
                <img src={Sketch} alt="">
                <h3>Quality 3</h3>
            </div>
            <div class="content">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore dolorem minima nobis accusantium animi nihil, id quo deleniti officiis illum rem magni ea adipisci iure atque magnam expedita? Facilis, pariatur.</p>
            </div>
        </div>
    </div>
</section>

  <style>
   
*
{
    margin:0;
    padding: 0;
    box-sizing: border-box;
}

.section.why{
    display:flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    min-height: 100vh;
    background-color: var(--mint-cream);
    overflow:hidden
}
.title{
    font-size: var(--fs-2); 
}
.container
{
    position:relative;
    width: 1050px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    transform: skewY(-10deg);
    margin-bottom: 90px;

}

.container .card:nth-child(1):before {
    content: "";
    position:absolute;
    top: -15px;
    left: 0;
    width: 100%;
    height: 15px;
    background: #161616;
    transform-origin:bottom;
    transform: skewX(45deg);
    transition: 0.5s;
}

.container .card:nth-child(1)::after{
    content: "";
    position:absolute;
    top: -15px;
    left: -15px;
    width: 15px;
    height: 100%;
    background: #d6d6d6;
    transform-origin:left;
    transform: skewY(45deg);
    transition: 0.5s;
    border-top: 200px solid #161616;
    
}
.container .card:nth-child(2):before {
    content: "";
    position:absolute;
    top: -15px;
    left: 0;
    width: 100%;
    height: 15px;
    background: #9b0101;
    transform-origin:bottom;
    transform: skewX(45deg);
    transition: 0.5s;
}

.container .card:nth-child(2)::after{
    content: "";
    position:absolute;
    top: -15px;
    left: -15px;
    width: 15px;
    height: 100%;
    background: #d6d6d6;
    transform-origin:left;
    transform: skewY(45deg);
    transition: 0.5s;
    border-top: 200px solid #9b0101;
    
}
.container .card:nth-child(3):before {
    content: "";
    position:absolute;
    top: -15px;
    left: 0;
    width: 100%;
    height: 15px;
    background: #b1ae09;
    transform-origin:bottom;
    transform: skewX(45deg);
    transition: 0.5s;
}

.container .card:nth-child(3)::after{
    content: "";
    position:absolute;
    top: -15px;
    left: -15px;
    width: 15px;
    height: 100%;
    background: #d6d6d6;
    transform-origin:left;
    transform: skewY(45deg);
    transition: 0.5s;
    border-top: 200px solid #b1ae09;
    
}
.container .card{
    position: relative;
    width: 300px;
    height: 400px;
    background: #fff;
    transition: 0.5s;
    cursor:default;
}
.container:hover .card:hover{
    transform: translateY(-40px);
}

.container .card:nth-child(1) .imgBx
{
    position: relative;
    width: 300px;
    height: 200px;
    background: #434343;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.container .card:nth-child(2) .imgBx
{
    position: relative;
    width: 300px;
    height: 200px;
    background: #ff0000;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.container .card:nth-child(3) .imgBx
{
    position: relative;
    width: 300px;
    height: 200px;
    background: #ffdd00;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.container .card .imgBx img{
    max-width: 100px;
}

.container .card .imgBx h3{
    position: relative;
    color: #fff;
    margin-top: 10px;
}

.container .card .content{
    position:relative;
    width:100%;
    height:200px;
    padding: 20px;
    color: #777;
    background:#fff ;
    text-align:center;
}

.container .card .content::before{
   content: "";
   position: absolute;
   left: 0;
   bottom: 0;
   width:100%;
   height: 400px;
   background:linear-gradient(transparent,transparent,rgba(0,0,0,.1)) ;
   transform-origin: bottom;
   transform: skewX(45deg) ;
   transition: 0.5s;
   pointer-events: none;
   z-index: -1;
}


.container .card:hover .content::before{
    transform: translateY(40px) skew(45deg) ;
    filter: blur(5px);
    opacity: 0.5;
}

.container.card:nth-child(3){
    z-index: 3;
    
}
.container.card:nth-child(2){
    z-index: 2;
}

.container.card:nth-child(1){
    z-index: 1;
}

@media (max-width: 994px) {
    body{
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: center;
    overflow:hidden;}
    .card {       
        width: 80%;
        margin-bottom: 50px;             
    }
    .container
    {
        display: flex;
        flex-wrap: nowrap;
        flex-direction: column;
        margin-right: 80px;
        align-items: center;
        padding-top: 100px;
        position: relative;
        left: 15%;   
        top:80%;
    }    
    .container .card
    {padding-bottom: 40px}

    .container .card:hover {
        transform: translateY(-25px);
    }
}
  </style>