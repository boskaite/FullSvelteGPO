<script>
	console.log("str2 started");
	let loging="";
	let password="";
</script>

<main>
	<div id="mainWindow">
		<h1 class="autorise">АВТОРИЗАЦИЯ</h1>
		<div id="square">
			<input class="pole" type="text" placeholder="Логин, номер телефона" value={loging}>
			<input class="pole" type="password" placeholder="Пароль" value={password}>
			<button class="autorization" onclick="location.href='http://localhost:8080/#/maincontrollpage'">Войти</button>
		</div>
		<p id="comment">По вопросам обращаться на почту: gpofvs@mail.ru</p>
	</div>
</main>

<style>
	main {
		width: 100%;
		height: 100%;
		margin: 0 auto;
	}
	#mainWindow {
		background-image: url(source/Фон.jpg);
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
		background-clip: content-box;
		height: 100%;
		width: auto;
	}
	.autorise{
		color: #DB0000;
		margin: 0;
		position: absolute;
		top: 10%;
		left: 10%;
		font-size: 72px;
	}
	#square {
		position: absolute;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding-top: 2%;
		left: 7%;
		top: 25%;
		width: 35%;
        height: 60%;
        border-radius: 65px;
		background: linear-gradient(#FF4400, #FFA800);
	}
	.pole {
		left: 10%;
		width: 80%;
		height: 15%;
		border-radius: 10px;
		border-style: none;
		color: #8D8D8D;
		font-size: large;
		margin-bottom: 5%;
	}
	.autorization {
		width: 50%;
		height: 15%;
		margin: 5%;
		background-color: #1D66F2;
		border-color: #1D66F2;
		color: white;
		font-size: 30px;
		font-weight: 700;
		cursor:pointer;
	}
	#comment{
		position: absolute;
		right: 3%;
		bottom: 15%;
		color: white;
		margin: 0;
		font-size: 20px;
	}
</style>

