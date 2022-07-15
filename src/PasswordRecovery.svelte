<script>
    console.log("str recovery started");
	let loging="";
</script>

<main>
    <div id="mainWindow">
        <div id="square">
            <h4>Восстановление пароля</h4>
            <p>Если Вы забыли свой пароль, введите свой логин или почту.</p>
            <input class="pole" type="text" placeholder="Логин, почта" value={loging}>
        </div>
        <button class="recovery" onclick="location.href='http://localhost:8080/#/warningEmail'">Продолжить</button>
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
		justify-content: center;
		align-items: center;
		width: 35%;
        height: 30%;
        padding: 2%;
        margin: 5%;
        border-radius: 30px;
		background: linear-gradient(#FF4400, #FFA800);
	}
    h4{
        color: white;
		margin: 10px;
		font-size: 35px;
        font-weight: 300;
    }
	.pole {
		width: 80%;
		height: 25%;
        margin-top: 20px;
		border-radius: 10px;
		border-style: none;
		color: #8D8D8D;
		font-size: large;
		margin-bottom: 5%;
	}
	.recovery {
		width: 20%;
		height: 7%;
		background-color: #1D66F2;
		border-color: #1D66F2;
		color: white;
		font-size: 30px;
		font-weight: 700;
		cursor:pointer;
	}
	p {
		color: white;
		margin: 10px;
		font-size: 20px;
	}
</style>