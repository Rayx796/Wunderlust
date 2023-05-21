
<svelte:head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</svelte:head>

	<footer>
		<div class="container">
			<div class="sec aboutus">
				<h2>About Us</h2>
				<p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Veniam ratione qui esse sed illo nam, sint ut exercitationem quam nesciunt.</p>
				<ul class="sci">
					<li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
					<li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
					<li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
					<li><a href="#"><i class="fa-brands fa-youtube"></i></a></li>
				</ul>
			</div>
			<div class="sec quicklinks">
				<h2>Support</h2>
				<ul>
					<li><a href="#">FAQ</a></li>
					<li><a href="#">Privacy Policy</a></li>
					<li><a href="#">Help</a></li>
					<li><a href="#">Contact</a></li>
				</ul>
			</div>
			<div class="sec quicklinks">
				<h2>Shop</h2><ul>
					<li><a href="#">Men</a></li>
					<li><a href="#">Women</a></li>
					<li><a href="#">Kids</a></li>
					<li><a href="#">Shoes</a></li>
				</ul>
			</div>
			<div class="sec contact">
				<h2>Contact Us</h2>
				<ul class="info">
					<li>
						<span><i class="fa-solid fa-phone"></i></span><p><a href="tel:+12345678900">+1 234 567 8900</a></p>
					</li>
					<li>
						<span><i class="fa-solid fa-envelope"></i></span><p><a href="mailto:knowmore@emailto.meee">wunderlust@emailto.meee</a></p>
					</li>
				</ul>
			</div>
		</div>
	</footer>
	<div class="copyrightText">
		<p>Copyright ©2023 Wunderlust. All Rights Reserved.</p>
	</div>

<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins:200,300,400,500,600,700,800,900&display=swap');
footer 
{
	position: relative;
	width: 100%;
	height: auto;
	padding: 50px 100px;
	background: #fff;
}
footer .container 
{
	width: 100%;
	display: grid;
	grid-template-columns: 2fr 1fr 1fr 1fr;
	grid-gap: 20px;
}
footer .container .sec h2 
{
	position: relative;
	color: #333;
	font-weight: 600;
	margin-bottom: 15px;
}
footer .container .sec p 
{
	color: #555;
}
footer .container .sci 
{
	margin-top: 20px;
	display: grid;
	grid-template-columns: repeat(4,50px);
}
footer .container .sci  li 
{
	list-style: none;
}
footer .container .sci  li a 
{
	display: inline-block;
	width: 36px;
	height: 36px;
	background: #333;
	display: grid;
	align-content: center;
	justify-content: center;
	text-decoration: none;
}
footer .container .sci  li a i 
{
	color: #fff;
	font-size: 20px;
}
footer .container .quicklinks
{
	position: relative;
}
footer .container .quicklinks ul li
{
	list-style: none;
}
footer .container .quicklinks ul li a 
{
	color: #555;
	text-decoration: none;
	margin-bottom: 10px;
	display: inline-block;
}
footer .container .contact .info 
{
	position: relative;
}
footer .container .contact .info li 
{
	display: grid;
	grid-template-columns: 30px 1fr;
	margin-bottom: 16px;
}
footer .container .contact .info li span 
{
	color: #555;
	font-size: 20px;
}
footer .container .contact .info li a 
{
	color: #555;
	text-decoration: none;
}
.copyrightText 
{
	width: 100%;
	background: #fff;
	padding: 20px 100px 30px;
	text-align: center;
	color: #555;
	border: 1px solid rgba(0,0,0,0.15);
}
@media (max-width: 991px)
{
	footer 
	{
    padding: 40px;
	}
	footer .container
	{
    width: 100%;
    display: grid;
    grid-template-columns: repeat(2,1fr);
    grid-gap: 20px;
	}
	.copyrightText
	{
		padding: 20px 40px 30px;
	}	
}
@media (max-width: 768px) 
{
	footer .container
	{
    width: 100%;
    display: grid;
    grid-template-columns: repeat(1,1fr);
    grid-gap: 20px;
	}
}
</style>