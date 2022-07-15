<script>
	console.log("str newPassword started");
	let loging="";
	let password="";
</script>

<main>
	<div id="mainWindow">
		<div id="square">
            <h4>Установка пароля</h4>
            <p>Введите новый пароль</p>
			<input class="pole" type="text" placeholder="   Новый пароль" value={loging}>
            <p>Подтвердите новый пароль</p>
			<input class="pole" type="password" placeholder="   Подтверждение пароля" value={password}>
		</div>
        <button class="newPassword">Сменить пароль</button>
	</div>
</main>

<style>
	main {
		width: 100%;
		height: 100%;
		margin: 0 auto;
	}
	#mainWindow {
		background-image: url(source/Фон1.jpg);
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
		background-clip: content-box;
		height: 100%;
		width: auto;
        display: flex;
		flex-direction: column;
		align-items: center;
	}
	#square {
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		align-items:center;
		width: 35%;
        height: 50%;
        margin: 5%;
        padding: 1%;
        border-radius: 60px;
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
		margin-bottom: 2%;
	}
     h4{
        color: white;
        margin: 1%;
		font-size: 35px;
        font-weight: 300;
    }
    p {
		color: white;
		margin: 10px;
		font-size: 20px;
	}
    .newPassword {
		width: 20%;
		height: 7%;
		background-color: #1D66F2;
		border-color: #1D66F2;
		color: white;
		font-size: 30px;
		font-weight: 700;
	}
</style>

