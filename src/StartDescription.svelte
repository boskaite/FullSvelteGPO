<script>
    
</script>

<main>
	<div id="mainWindow">
		<div id="discription">
			<h1>SMART HOME</h1>
			<h2>Система управления электричеством в вашем доме.</h2>
			<p>Дистанционный контроль параметров сети электропитания, управление подачи электричества по линиям электросети, исторические данные по электросетити.</p>
            <button class="autorization" onclick="location.href='http://localhost:8080/#/autorization'">АВТОРИЗАЦИЯ</button>
        </div>
        <div>
            <p id="comment">По вопросам обращаться на почту: gpofvs@mail.ru</p>
        </div>
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
	#discription {
		position: absolute;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        top: 5%;
		left: 10%;
		width: 30%;
        height: 90%;
	}
	h1 {
		color: #DB0000;
		text-align:center;
		margin: 0;
		font-size: 4em;
	}
	h2, p {
		color: #505050;
		font-size: 1.3em;
		margin: 15px;
	}
	.autorization {
		width: 80%;
		height: 8%;
        margin-top: 5%;
		background-color: #DB0000;
		border-radius: 15px;
        border-style: none;
		color: white;
		font-size: 1em;
		font-weight: 700;
		cursor:pointer;
	}
	.autorization:hover {
		background-color:#ff9c01;
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