
<section>
	<div class="bg"></div>
	<div class="bg"></div>
	<div class="card">
		<img src="./bg-pattern-card.svg" alt="top" class="img-top">
		<img src="./image-victor.jpg" alt="Victor" class="person">
		<h2 class="victor">Victor Crest<span>26</span></h2>
		<h4>London</h4>
		<ul>
			<li><h2 class="my-list">80K</h2><p>Followers</p></li>
			<li><h2 class="my-list">803K</h2><p>Likes</p></li>
			<li><h2 class="my-list">1.4K</h2><p>Photos</p></li>
		</ul>
	</div>
</section>

<style>

	@import url('https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@400;700&display=swap');

	*{
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		font-family: 'Kumbh Sans', sans-serif;
	}
	:global(body){
		margin: 0;
		padding: 0;
		display: flex;
		justify-content: center;
		align-items: center;		
	}
	section{
		position: relative;
		display: flex;
		justify-content: center;
		align-items: center;
		width: 1440px;
		height: 800px;		
		background: linear-gradient(63.18deg, #19A2AE 0%, #2D3248 100%);
	}

	.bg:nth-child(1){
		position: absolute;
		transform: rotate(180deg);
		top: 0;
		left: 0;
		width: 40vw;
		height: 50vh;
		background-image: url(../bg-pattern-top.svg);
	}
	.bg:nth-child(2){
		position: absolute;
		bottom: 0;
		right: 0;
		width: 40vw;
		height: 50vh;
		background-image: url(../bg-pattern-bottom.svg);
	}
	.card{
		position: relative;
		display: grid;
		grid-template-rows: 140px 140px 1fr ;
		background: white;		
		border-radius: 15px;
		width: 350px;
		height: 370px;				
	}
	.card .img-top{
		grid-row: 1;
		border-top-left-radius: 15px;
		border-top-right-radius: 15px;
	}
	.card .person{
		position: absolute;
		grid-row: 1/3;
		justify-self: center;
		align-self: center;
		border-radius: 50%;
		border: solid 5px white;
					
	}
	.card .victor{
		position: absolute;
		grid-row: 2/3;
		justify-self: center;
		align-self: center;
		font-size: 18px;
		margin-top: 1.5em;
	}
	.card span{
		position: relative;
		grid-row: 2/3;
		align-self: center;
		font-size: 18px;
		color: gray;
		font-weight: 300;
		margin-left: 5px;
	}
	.card h4{
		position: relative;
		grid-row: 2/3;
		justify-self: center;
		align-self: center;		
		color: gray;
		font-weight: 100;		
		margin-top: 6em;
		font-size: 14px;
	}
	.card ul{
		position: relative;		
		grid-row: 3/4;
		display: flex;
		justify-content: space-around;
		border-top: solid 1px rgba(148, 148, 148, 0.24);
		align-items: center;
		padding: 0 1.5em ;						
	}

	.card ul li{
		position: relative;
		display: inline-block;
		text-decoration: none;
		text-align: center;				
	}
	.my-list{
		font-size: 18px;
		transform: scale(1.2, 1);
	}	
	p{
		 color: gray;
		 font-size: 11px;
		 letter-spacing: 2px;
		 margin-top: 0.4em;
	}


</style>