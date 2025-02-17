<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Солнечная система</title>
<style>
    .solar-system {
    width: 1000px;
    height: 1000px;
    margin: auto;
    position: relative;
    border: 1px solid #000;
    border-radius: 50%;
    overflow: hidden;
}

.sun {
    width: 60px;
    height: 60px;
    background-color: #ffd700;
    border-radius: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 9;
}

.orbit {
    margin-top: 12px;
    width: 100%;
    height: 100%;
    transform-origin: center;
    animation: orbit 10s linear infinite;
}

.planet {
    width: 15px;
    height: 15px;
    background-color: #808080;
    border-radius: 50%;
    position: absolute;
    top: 0;
    left: 0;
    transform-origin: center;
}

.mercury-orbit {
    animation-duration: 5s;
}

.venus-orbit {
    margin-top: -1010px;
    animation-duration: 8s;
}

.earth-orbit {
    margin-top: -985px;
    animation-duration: 13s;
}

.mars-orbit {
    margin-top: -990px;
    animation-duration: 9s;
}

.jupiter-orbit {
    margin-top: -995px;
    animation-duration: 20s;
}

.saturn-orbit {
    margin-top: -1005px;
    animation-duration: 10s;
}

.uranus-orbit {
    margin-top: -1010px;
    animation-duration: 12s;
}

.neptune-orbit {
    margin-top: -1000px;
    animation-duration: 15s;
}

@keyframes orbit {
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(360deg);
    }
}


.mercury {
    background-color: #bdb76b;
    width: 12px;
    height: 12px;
    top: calc(50% - 45px);
    left: calc(50% + 45px);
}

.venus {
    background-color: #c19a6b;
    width: 14px;
    height: 14px;
    top: calc(50% - 55px);
    left: calc(50% + 55px);
}

.earth {
    background-color: #4682b4;
    width: 16px;
    height: 16px;
    top: calc(50% - 65px);
    left: calc(50% + 65px);
}

.mars {
    background-color: #cd5c5c;
    width: 18px;
    height: 18px;
    top: calc(50% - 100px);
    left: calc(50% + 100px);
}

.jupiter {
    background-color: #daa520;
    width: 32px;
    height: 32px;
    top: calc(50% - 150px);
    left: calc(50% + 150px);
}

.saturn {
    background-color: #dda0dd;
    width: 28px;
    height: 28px;
    top: calc(50% - 200px);
    left: calc(50% + 200px);
}

.uranus {
    background-color: #00ffff;
    width: 26px;
    height: 26px;
    top: calc(50% - 250px);
    left: calc(50% + 250px);
}

.neptune {
    background-color: #00008b;
    width: 24px;
    height: 24px;
    top: calc(50% - 300px);
    left: calc(50% + 300px);
}

</style>
</head>
<body>
    <div class="solar-system">
        <div class="sun"></div>
        <div class="orbit mercury-orbit">
            <div class="planet mercury"></div>
        </div>
        <div class="orbit venus-orbit">
            <div class="planet venus"></div>
        </div>
        <div class="orbit earth-orbit">
            <div class="planet earth"></div>
        </div>
        <div class="orbit mars-orbit">
            <div class="planet mars"></div>
        </div>
        <div class="orbit jupiter-orbit">
            <div class="planet jupiter"></div>
        </div>
        <div class="orbit saturn-orbit">
            <div class="planet saturn"></div>
        </div>
        <div class="orbit uranus-orbit">
            <div class="planet uranus"></div>
        </div>
        <div class="orbit neptune-orbit">
            <div class="planet neptune"></div>
        </div>
    </div>
</body>
</html>
