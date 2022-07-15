<script>
    console.log("str email started");
</script>

<main>
    <div id="mainWindow">
        <div id="square">
            <h4>Проверьте почту</h4>
            <p>На вашу почту, которая привязана к вашей учетной записи, была выслана инструкция по завершению сброса пароля.</p>
            <p>Если в течении ближайших минут письмо с инструкциями не появится в папке с входящими письмами, проверьте папку "Спам".</p>
        </div>
        <button class="ready">Готово</button>
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
	.ready {
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