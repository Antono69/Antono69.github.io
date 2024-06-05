<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="utf-8">
        <title>proyecto 2</title>
        <style>
            body{
                background: linear-gradient(120deg, #906bff, #57eaff);
                font-family: 'Arial Nova', sans-serif;
            }
            h1{
                text-align: center;
                color: 	#4B0082
            }
            article{
                padding: 1em;
                position: absolute;
                left: 58%;
                border: solid;
                border-radius: 3em;
            }
            h3{
                font-size: 1.7em;
            }
            .come{
                font-size: 1.3em;
                color: black;
            }
            .res{
                color: midnightblue;
                font-size: 1.18em;
            }
            .tab{
                color: aqua;
                border: solid 0.2em purple;
            }
            h2{
                color: 	#4B0082;
            }
            .parrafo{
                max-width: 500px;
                text-align: left;
            }
            .img{
                height: 15em;
                width: 15em;
                display: inline-block;
            }
        </style>
    </head>
    <body>
        <h1><strong>VOLEYBOOL</strong></h1>
        <article>
            <h3>¿que opinas sobre el deporte?</h3>
            <form method="post" action="proyectoo2.php">
                <h3>deja tu comentario de que opinas</h3><input type="text" name="com"/><br>
                <input type="submit" value="deja tu comentario"/>
            </form>
            <?php
$xml = simplexml_load_file('proyecto2xml.xml');

if(isset($_POST["com"])){
    $com = $_POST["com"];
    $opinion = $xml->addChild('opinion');
    $opinion->addChild('comentario', $com);
    $xml->asXML('proyecto2xml.xml');
}

$t = count($xml->opinion);
if($t > 0){
    echo "<table border=1 class='tab'>";
    for ($i = 0; $i < $t; $i++){
        $o = $xml->opinion[$i];
        echo "<tr>";
        echo "<td class='come'>Comentario $i</td>";
        echo "<td class='res'>" . $o->comentario . "</td>";
        echo "</tr>";
    }
    echo "</table>";
} else {
    echo "No hay comentarios aún.";
}
?>
        </article>
        <h2>Introducción</h2>
        <h4 class="parrafo">en esta pagina web veras un poco de lo que es mi gusto por el voleybol que es deporte que a mi me gusta mucho que ademas práctico.Si te a ti también te gusta, sabes algo del deporte o después de ver esta pagina te gusta, puedes deja una comentario en la parte de la derecha sonre que opinas sobre este deporte</h4>
        <h2>¿QUE ES EL VOLEYBOOL?</h2>
        <h4 class="parrafo">es un deporte donde dos equipos se enfrentan sobre un terreno de juego liso separados por una red central, tratando de pasar el balón por encima de la red hacia el suelo del campo contrario.</h4>
        <h2>COMO SE JUEGA</h2>
        <h4 class="parrafo"> El voleibol es un deporte de equipo que se juega entre dos equipos de seis jugadores cada uno. El objetivo principal del juego es enviar el balón por encima de la red y hacer que toque el suelo en el campo del equipo contrario, mientras que el otro equipo intenta evitar que el balón toque suelo en su lado.</h4>
        <ol type="1" class="parrafo">
            <li><strong>EL campo</strong>: El campo de voleibol está dividido en dos partes iguales por una red. Cada lado del campo tiene unas dimensiones específicas.</li>
            <li><strong>Inicio del juego</strong>: El juego comienza con un saque. El equipo que sirve el balón lo hace desde detrás de la línea de fondo de su campo.</li>
            <li><strong>Pases</strong>: Los jugadores pueden pasar el balón entre ellos usando golpes como el pase de antebrazo, el saque de volea o el toque de dedos. El objetivo es mantener el control del balón y preparar para un ataque.</li>
            <li><strong>Ataque</strong>: Cuando el balón se encuentra cerca de la red, los jugadores pueden intentar atacar golpeándolo con fuerza hacia el campo contrario. Esto se hace generalmente mediante un remate o un bloqueo.</li>
            <li><strong>Bloqueo</strong>: Los jugadores pueden intentar bloquear los ataques del equipo contrario saltando cerca de la red con las manos extendidas para interceptar el balón.</li>
            <li><strong>Fuera de juego</strong>: El balón se considera fuera de juego si aterriza fuera de los límites del campo, toca el techo o las estructuras que lo rodean, o si pasa por debajo de la red.</li>
        </ol>
        <h2>Imagenes</h2>
        <img src="1.jpg" class="img">
        <img src="2.jpg" class="img">
        <img src="3.jpg" class="img">
        <img src="4.jpg" class="img">
    </body>
    
</html>
