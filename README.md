<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html>
    <head style="right: ">
        <!--<meta charset="UTF-8">-->
        <title>Mail Form</title>
        <link rel="stylesheet" type="text/css" href="estilo.css">
    </head>
    <body background="montañas.jpg"><br>
    <center><h1 style="color: whitesmoke">NUEVO MUNDO</h1>
        <h5 style="color: white">"Bienvenido a la Educacion del Futuro"</h5><br></center>   
    <form action="" method="post">
        <input type="text" placeholder="Nombre" name="txtnombre">
        <input type="text" placeholder="Apellidos" name="txtapellidos">
        <input type="text" placeholder="Telefono" name="txttelefono">
        <textarea placeholder="email" name="txtemail"></textarea>
        <input type="submit" value="R E G I S T R A R">
    <!--<center>
        <h1 style="color: whitesmoke">NUEVO MUNDO</h1>
        <h5 style="color: white">"Bienvenido a la Educacion del Futuro"</h5><br><br><br>
        <h1 style="color: whitesmoke">R E G I S T R A T E</h1>
        <p><input type="text"  name="txtnombres" value="Nombre:" size="90" style="background-color: lightskyblue;color: gray;width: 600px;height: 30px"></p>
        <p height="90px"><input type="text"  name="txtapellidos" value="Apellidos:" style="background-color: lightskyblue;color: gray;width: 600px;height: 30px"></p>
            <p height="90px"><input type="text"  name="txttelefono" value="Teléfono:" size="90"style="background-color: lightskyblue;color: gray;width: 600px;height: 30px"></p>
            <p height="90px"><input type="text"  name="txtemail" value="Email:" size="90"style="background-color: lightskyblue;color: gray;width: 600px;height: 30px"></p></p>
    
        <input type="submit" name="btnenviar" value="REGISTRAR" style="background-color: dodgerblue; color: white;width: 400px;height: 30px">
       
    
    </center>-->
            
     </form>
        <?php
        $nomb = filter_input(INPUT_POST,'txtnombres');
        $apell = filter_input(INPUT_POST,'txtapellidos');
        $tel = filter_input(INPUT_POST,'txttelefono');
        $email = filter_input(INPUT_POST,'txtemail');
        $mail = @mail($email, $nomb, $apell,$tel)
        ?>
        
    </body>
</html>
