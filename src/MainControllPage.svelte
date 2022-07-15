<script>
let name="Мария";
</script>

<main>
	<div id="mainWindow">
        <div id="upBackground"></div>
        <div id="content">
            <div id="headMenu">
                <div>
                    <h3>Добро пожаловать домой, {name}</h3>
                    <h5>//день недели, дата//</h5>
                    <h5>//время//</h5>
                </div>
                <div id="personCabinet" onclick="location.href='http://localhost:8080/#/personinform'">
                    <div id="iconCabinet"></div>
                    <h3 id="personName">{name}</h3>
                </div>
            </div>
            <div id="bodyPage">
                <div class="square" id="controll">
                    <div class="textControll">
                        <h4>Линия №1</h4>
                        <div class="swich"></div>
                        <h4>Линия №2</h4>
                        <div class="swich"></div>
                    </div>
                </div>
            </div>
        </div>
	</div>
</main>

<style>
	main {
		width: 100%;
		height: 100%;
		margin: 0 auto;
	}
    h3 {
        color:#FF5C00;
        font-size: 32px;
        margin: 0;
        opacity: 1;
    }
    h5{
        color: #1D66F2;
        font-size: 18px;
        margin: 0;
    }
    h4{
        color: black;
    }
	#mainWindow {
		background-image: url(source/Фон1.jpg);
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
		background-clip: content-box;
		height: 100%;
		width: auto;
	}
    #upBackground{
        position: absolute;
        width: 100%;
        height: 100%;
        background: rgba(255, 255, 255, 0.5);
    }
    #content{
        position:absolute;
        width: 100%;
        height: 100%;
    }
    #headMenu{
        display: flex;
        justify-content: space-between;
        width: 90%;
        margin-left: 5%;
        padding-top: 3%;
    }
    #personCabinet{
        display: flex;
        flex-direction: row;
        align-items: center;
        height:5%;
        cursor:pointer;
    }
    #iconCabinet{
        width: 2em;
        height: 2em;
        background-image: url(source/icon.svg);
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
    }
    #bodyPage{
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        margin: 2%;
        z-index: 10;
    }
	.square {
        padding: 1%;
        border-radius: 60px;
		background: #FF5C00;
        opacity: 0.2;
	}
    #controll{
        display: flex;
		flex-direction: column;
		justify-content: space-around;
		align-items:center;
		width: 35%;
        height: 50%;
    }
</style>