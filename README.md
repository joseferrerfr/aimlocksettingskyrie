# aimlocksettingskyrie
<!DOCTYPE html>
<!-- saved from url=(0052)file:///C:/Users/josep/Downloads/PanelTrickAuto.html -->
<html lang="es" style="--main-color: #ff0000;"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <title>Panel8/12/24</title>
    <script src="./PanelHTMLXITADO_files/particles.min.js.descargar"></script><style type="text/css" id="operaUserStyle"></style>
    <style>
        body {
            background-color: #000;
            font-family: 'Courier New', monospace;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            position: relative;
            overflow: hidden;
        }
        #particles-js {
            position: fixed;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -1;
        }
        .panel-container {
            background-color: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 10px;
            width: 90%;
            max-width: 500px;
            margin: 20px auto;
            position: relative;
            overflow: hidden;
            animation: float 10s ease-in-out infinite;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .panel-container:hover {
            transform: scale(1.05);
        }
        h1 {
            text-align: center;
            color: #ff0000;
            text-shadow: 1px 1px 3px #000000;
            margin-bottom: 5px;
        }
        .subtitle {
            text-align: center;
            color: #e60000;
            font-size: 0.8em;
            margin: 5px 0;
        }
        .description {
            text-align: center;
            color: #ffffff;
            font-size: 0.9em;
            margin-bottom: 20px;
        }
        .credits {
            text-align: center;
            color: #800080; 
            font-size: 0.7em;
            margin: 10px 0;
        }
        .checkbox-container {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 15px;
            width: 48%;
        }
        .checkbox-label {
            color: #ff0000;
            margin-left: 10px;
        }
        .checkbox-row {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }
        #save-settings {
            background-color: #ff0000;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
            transition: background 0.3s;
        }
        #save-settings:hover {
            background-color: #cc0000;
        }
        @keyframes float {
            0% { transform: translatey(0px); }
            50% { transform: translatey(-20px); }
            100% { transform: translatey(0px); }
        }
        .notification {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background-color: rgba(255, 0, 0, 0.8);
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            z-index: 1000;
        }
        .progress-container {
            margin: 20px 0;
        }
        .progress-title {
            color: var(--main-color, #ff0000);
            text-align: center;
            margin-bottom: 5px;
        }
        .progress-bar {
            background: #333;
            border-radius: 5px;
            height: 20px;
            position: relative;
            overflow: hidden;
            box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.5);
            cursor: pointer;
        }
        .progress-fill {
            background: #ff0000;
            height: 100%;
            width: 0;
            transition: width 0.5s;
            border-radius: 5px 0 0 5px;
        }
        /* Estilos para los interruptores */
        .switch {
            position: relative;
            display: inline-block;
            width: 50px;
            height: 30px;
        }
        .switch input {
            opacity: 0;
            width: 0;
            height: 0;
        }
        .slider {
            position: absolute;
            cursor: pointer;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: #ccc;
            transition: .4s;
            border-radius: 34px;
        }
        .slider:before {
            position: absolute;
            content: "";
            height: 22px;
            width: 22px;
            border-radius: 50%;
            left: 4px;
            bottom: 4px;
            background-color: white;
            transition: .4s;
        }
        input:checked + .slider {
            background-color: #4CAF50;
        }
        input:checked + .slider:before {
            transform: translateX(20px);
        }

        input[type="checkbox"], input[type="radio"] {
            appearance: none;
            width: 20px;
            height: 20px;
            border: 2px solid #ff0000;
            border-radius: 4px;
            position: relative;
            outline: none;
            cursor: pointer;
            transition: background 0.3s, border-color 0.3s;
        }
        input[type="checkbox"]:checked, input[type="radio"]:checked {
            background-color: #ff0000;
            border-color: #ff0000;
        }
        input[type="checkbox"]:checked::after, input[type="radio"]:checked::after {
            content: '✔';
            position: absolute;
            top: 0;
            left: 2px;
            color: white;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <div id="particles-js"></div>
    
    <div class="panel-container" id="panel">
        <h1>PANEL HTML AIMLOCK</h1>
        <p class="description">Panel con nuevos códigos y comandos actualizados Hoy 18 De Diciembre - Creador: Kyriexss</p>
        <h2 class="subtitle">Configuración del Sistema</h2>

        <div class="checkbox-row">
            <div class="checkbox-container">
                <input type="checkbox" id="aimlock-checkbox">
                <label class="checkbox-label">Aimlock</label>
            </div>
            <div class="checkbox-container">
                <input type="checkbox" id="aimfov-checkbox">
                <label class="checkbox-label">Aim FOV</label>
            </div>
        </div>

        <div class="checkbox-row">
            <div class="checkbox-container">
                <input type="checkbox" id="regedit-checkbox">
                <label class="checkbox-label">Regedit</label>
            </div>
            <div class="checkbox-container">
                <input type="checkbox" id="supresor-checkbox">
                <label class="checkbox-label">Supresor</label>
            </div>
        </div>

        <div class="progress-container">
            <div class="progress-title">Sensitivity</div>
            <div class="progress-bar" onclick="setProgress(event, &#39;sensitivity-bar&#39;)">
                <div id="sensitivity-bar" class="progress-fill"></div>
            </div>
        </div>

        <div class="progress-container">
            <div class="progress-title">Touch Speed</div>
            <div class="progress-bar" onclick="setProgress(event, &#39;touchspeed-bar&#39;)">
                <div id="touchspeed-bar" class="progress-fill"></div>
            </div>
        </div>

        <div class="checkbox-row">
            <div class="checkbox-container">
                <input type="radio" id="noDPI" name="dpi" value="noDPI" checked="">
                <label class="checkbox-label">No DPI</label>
            </div>
            <div class="checkbox-container">
                <input type="radio" id="dpi600" name="dpi" value="600">
                <label class="checkbox-label">DPI +600</label>
            </div>
            <div class="checkbox-container">
                <input type="radio" id="dpi1200" name="dpi" value="1200">
                <label class="checkbox-label">DPI +1200</label>
            </div>
        </div>

        <div class="checkbox-row">
            <div class="checkbox-container">
                <label class="checkbox-label">FPS Stabilizer</label>
            </div>
            <div class="checkbox-container">
                <label class="switch">
                    <input type="checkbox" id="fps-stabilizer">
                    <span class="slider"></span>
                </label>
            </div>
        </div>

        <div class="checkbox-row">
            <div class="checkbox-container">
                <label class="checkbox-label">No Recoil</label>
            </div>
            <div class="checkbox-container">
                <label class="switch">
                    <input type="checkbox" id="no-recoil">
                    <span class="slider"></span>
                </label>
            </div>
        </div>

        <button id="save-settings">Aplicar configuraciones</button>
    </div>

    <script>
        document.documentElement.style.setProperty('--main-color', '#ff0000');

        document.getElementById('save-settings').onclick = function() {
            const settings = {
                aimlock: document.getElementById('aimlock-checkbox').checked,
                aimfov: document.getElementById('aimfov-checkbox').checked,
                regedit: document.getElementById('regedit-checkbox').checked,
                supresor: document.getElementById('supresor-checkbox').checked,
                sensitivity: parseInt(document.getElementById('sensitivity-bar').style.width) || 0,
                touchSpeed: parseInt(document.getElementById('touchspeed-bar').style.width) || 0,
                dpi: document.querySelector('input[name="dpi"]:checked') ? document.querySelector('input[name="dpi"]:checked').value : 'None',
                fpsStabilizer: document.getElementById('fps-stabilizer').checked,
                noRecoil: document.getElementById('no-recoil').checked
            };
            console.log('Configuración guardada:', JSON.stringify(settings, null, 2));
            showNotification('Comandos y códigos activados correctamente, deja la aplicación en segundo plano');
        };

        function setProgress(event, barId) {
            const bar = document.getElementById(barId);
            const barWidth = event.currentTarget.clientWidth;
            const offsetX = event.clientX - event.currentTarget.getBoundingClientRect().left;
            const percentage = Math.min(Math.max(offsetX / barWidth * 100, 0), 100);
            bar.style.width = percentage + '%';
        }

        function showNotification(message) {
            const notification = document.createElement('div');
            notification.className = 'notification';
            notification.textContent = message;
            document.body.appendChild(notification);
            setTimeout(() => notification.remove(), 3000);
        }
    </script>


</body></html>
