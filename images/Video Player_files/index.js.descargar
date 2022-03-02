const $video = document.querySelector("#video")
const $play = document.querySelector("#play")
const $pause = document.querySelector("#pause")
const $backward = document.querySelector("#backward")
const $forward = document.querySelector("#forward")

//,,<BR
$play.addEventListener("click", handlePlay )
$pause.addEventListener("click", handlePause )

function handlePlay() {
    $video.play()
    $play.hidden = true
    $pause.hidden = false
    console.log("Le diste click al boton de reproducir")

    
}

function handlePause() {
    $video.pause()
    $play.hidden = false
    $pause.hidden= true
    console.log("Le diste click al boton de pausa")
}

$backward.addEventListener("click", handleBackward)

function handleBackward() {
    $video.currentTime = $video.currentTime-10
    console.log("Para atras 10sec", currentTime)

}

$forward.addEventListener("click", handleForward)

function handleForward() {
   $video.currentTime = $video.currentTime+10   
    console.log("Para adelante 10sec", currentTime)

}

/*<h1 class="txt1" id="tittle">HOLA MUNDO!</h1>
<h2 class="txt" id="subtittle">Primer intento de pagina web </h2>
<p class="txt">Reproduccion de video musical a traves <br> de botones programados desde
<br>Javascript y diseño a partir de CSS<br><p>
<h3 class="txt" id="question">¿Que es Javascript?</h3>
<p class="txt">JavaScript es el lenguaje de programación que debes usar para añadir características interactivas <br>a tu sitio web, (por ejemplo, juegos, eventos que ocurren cuando los botones son presionados o los <br> datos son introducidos en los formularios, efectos de estilo dinámicos, animación, y mucho más).</p>
*/

const $progress= document.querySelector("#progress")
$video.addEventListener("loadedmetadata", handleLoaded)
$video.addEventListener("timeupdate", handleTimeUpdate)


function handleLoaded() {
    console.log($video.duration)
    $progress.max = $video.duration
}

function handleTimeUpdate() {
    $progress.value=$video.currentTime
    console.log("Tiempo actual", $video.currentTime)
}

$progress.addEventListener("input", handleInput)

function handleInput() {
    $video.currentTime=$progress.value
    console.log($progress.value)
}



