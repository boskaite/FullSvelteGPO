<script>
	let fullName="Пикуль";
    let name="Мария";
    let patronymic="Александровна";
    let adress="Россия, г.Томск, ул. Вершинина 74, дом 4, кв. 5";
    let phoneNumber="+78967849897";
    let password="123456789";
    let newpassword;
    let repeadpassword;
</script>

<main>
    <div id="mainWindow">
        <div id="back">
            <div id="arrow" onclick="location.href='http://localhost:8080/#/personinform'"></div>
        </div>
        <div id="square">
            <div id="information">
                <div class="informCounts" id="text">
                    <p>Фамилия</p>
                    <p>Имя</p>
                    <p>Отчество</p>
                    <p>Адрес</p>
                    <p>Номер телефона</p>
                    <br/>
                    <p>Старый пароль</p>
                    <p>Новый пароль</p>
                    <p>Подтверждение пароля</p>
                </div>
                <div class="informCount" id="stroka">
                    <input class="pole" type="text" value={fullName}>
                    <input class="pole" type="text" value={name}>
                    <input class="pole" type="text" value={patronymic}>
                    <input class="pole" type="text" value={adress}>
                    <input class="pole" type="text" value={phoneNumber}>
                    <br/>
                    <input class="pole" type="password" value={password} readonly>
                    <input class="pole" type="password" value={newpassword} pattern="[A-Za-z0-9.,!]+">
                    <input class="pole" type="password" value={repeadpassword} pattern="[A-Za-z0-9.,!]+">
                </div>
            </div>
            <div id="button">
                <button class="recovery" onclick="location.href='http://localhost:8080/#/personinform'">
                    Изменить
                </button>
            </div>
        </div>
        <div id="personCabinet">
            <div id="iconCabinet"></div>
            <h3 id="personName">{name}</h3>
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
		background-image: url(source/Фон1.jpg);
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
		background-clip: content-box;
		height: 100%;
		width: auto;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
	}
    #back {
        width: 10%;
        height: 50%;
        margin-top: 5%;
    }
    #arrow{
        width: 0; 
        height: 0;
        border-top: 2em solid transparent;
        border-right: 2em solid #FF5C00;
        border-bottom: 2em solid transparent;
        cursor:pointer;
    }
	#square {
		display: flex;
		flex-direction: column;
		align-items: center;
		width: 55%;
        height: 75%;
        padding: 2%;
        padding-top: 5%;
        margin-top: 2.5%;
        border-radius: 30px;
		background: white;
	}
    #information{
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        width: 100%;
    }
    .informCount{
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        width: 50%;
    }
    input:invalid {
	    border:1px solid red;
    }
    #text{
        width: 30%;
    }
    #stroka{
        padding-top: 2%;
        width: 70%;
    }
   	p {
		margin: 5%;
        margin-bottom: 11%;
		font-size: 20px;
	}
	.pole {
		width: 90%;
		height: 7%;
		font-size: large;
		margin-bottom: 5%;
        border-color: #838383;
        border-style: solid;
        border-width: 1px;
	}
    #button {
        width: 100%;
        height: 8%;
        display: flex;
        justify-content: center;
        cursor:pointer;
    }
	.recovery {
		width: 30%;
		height: 100%;
        margin-top: 2%;
		background-color: #7082A6;
		border-color: #7082A6;
		color: white;
		font-size: 30px;
		font-weight: 700;
		cursor:pointer;
	}
     #personCabinet{
        display: flex;
        flex-direction: row;
        align-items: center;
        height:5%;
        margin-top: 3.2%;
        margin-right: 1.6%;
    }
    #iconCabinet{
        width: 2em;
        height: 2em;
		background-image: url(source/icon.svg);
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
    }
    h3 {
        color:#FF5C00;
        font-size: 32px;
        margin: 0;
        opacity: 1;
    }
</style>