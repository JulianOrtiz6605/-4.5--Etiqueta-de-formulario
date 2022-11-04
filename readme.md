           <!--          ¡CAMPO FORMULARIO!
    ⇒ <form> es la etiqueta principal para el formulario
    ⇒ <fieldset> </fieldset> No es una etiqueta obligatoria, esta etiqueta marca un cuadro que envuelve el formulario.
    ⇒ <legend>Título</legend> Para agregar un titulo al formulario.
    ⇒ <input> Este es el campo que el usuario va a diligenciar.
    ⇒ type="text" Este atribuo indica que tipo de contenido puede ingresar el usuario, en este ejemplo es de texto.
    ⇒ name="nombre" Este atributo es para darle información al servidor sobre lo que trata el campo del formulario.
    ⇒ id="camponombre" Para dar un identificador único al imput.
    ⇒ placeholder="Escribe tu nombre:" Agrega un texto de ayuda que desaparece al escribir en el campo.
    ⇒ value="Escribe tu nombre" El campo aparecerá dilienciado con el texto que escribamos en el atributo.
    ⇒ <label for=" "> </label> La etiqueta label va siempre acomplañada de un atributo for que conecta el nombre con el
     campo del imput. 
    ⇒ El label lo relacionamos con el id que en el ejemplo es camponombre, se recomienda que los id y nombre sean todos
     en minúscula para no tener difuculates al momento de relacionarlos, en el ejemplo hace que cuando le damos clik
     a nombre el cursor se va para el campo de escritura. 
    ⇒ disabled Este atribuo desabilita el campo se puede usar para condicionales.
    ⇒ max y min en campos numericos para limitar, ver ejemplo numvero2.
    ⇒ autofocus Este atribuo situa el cursor en el campo de escritura sin necesidad de dar click en el campo, no tiene valor.
    ⇒ required Este atribuo exige que se escriba el valor requerido en el campo, este atributo no tiene valor.

    CODIGO
<form>
        <fieldset>
                <legend>Formulario</legend>
                <!-- Campo de texto -->
                <p> <h5>Tiene un maxlength="6" para que solo ingresen 6 caracteres</h5>
                    <label for="camponombre">Nombre:</label>
                    <input type="text" name="nombre" id="camponombre" placeholder="Escribe tu nombre" maxlength="6">
                <hr>
                <p>Ejemplo con el atributo value=" " El usuario debe borrar si desea agregar texto diferente.</p>
                    <label for="camponombre">Nombre:</label>
                    <input type="text" name="nombre" id="camponombre-1" value="Escribe tu nombre"> 
                </p>
                <!-- ///////////// -->
                
                <!-- Campo de la contraseña -->
                <p>
                    <label for="password">Contraseña:</label>
                    <input type="password" name="password" id="password">
                </p>
                <!-- ////////////////////// -->

                <!-- Campo email-->
                <p> <h5>Email con ayuda de placeholder</h5>
                    <label for="email">Email:</label>
                    <input type="email" name="email" id="email" placeholder="email@dominio.com">
                </p>
                <!-- ///////////-->

                <!-- Campo fecha-->
                <p>
                    <label for="fecha">Fecha:</label>
                    <input type="date" name="fecha" id="fecha">
                </p>
                <!-- ///////////-->

                <!-- Campo fecha y hora-->
                <p>
                    <label for="fecha-hora">Fecha y hora:</label>
                    <input type="datetime-local" name="fecha-hora" id="fecha-hora">
                </p>
                <!-- ///////////-->

                <!-- Campo para subir archivos-->
                <p>
                    <label for="archivo">Subir archivo:</label>
                    <input type="file" name="archivo" id="archivo">
                </p>
                <!-- ///////////-->

                <!-- Campo mes-->
                <p>
                    <label for="mes">Mes:</label>
                    <input type="month" name="mes" id="mes">
                </p>
                <!-- ///////////-->

                <!-- Campo semana-->
                <p>
                    <label for="week">Semana:</label>
                    <input type="week" name="week" id="week">
                </p>
                <!-- ///////////-->

                 <!-- Campo teléfono -->
                 <p>
                    <label for="hora">Hora:</label>
                    <input type="time" name="hora" id="hora">
                </p>
                <!-- ///////////-->

                <!-- Campo número-->
                <p>
                    <label for="numero">Número:</label>
                    <input type="number" name="numero" id="numero">
                </p>
                <!-- ///////////-->

                <!-- Campo número con max y min-->
                <p> <h5>Max de 5 y min de 2</h5>
                    <label for="numero2">Número2:</label>
                    <input type="number" name="numero2" id="numero2" max="5" min="2">
                </p>
                <!-- ///////////-->

                <!-- Campo número conteo de 3 3n 3-->
                <p> <h5>Campo numerico y conteo de 3 en 3</h5>
                    <label for="numero3">Número3:</label>
                    <input type="number" name="numero3" id="numero2" step="3">
                </p>
                <!-- ///////////-->

                <!-- Campo rango -->
                <p>
                    <label for="rango">Rango:</label>
                    <input type="range" name="rango" id="rango">
                </p>
                <!-- ///////////-->

                <!-- Campo buscar -->
                <p>
                    <label for="buscar">Buscar:</label>
                    <input type="search" name="buscar" id="buscar">
                </p>
                <!-- ///////////-->

                <!-- Campo teléfono -->
                <p>
                    <label for="telefono">Teléfono:</label>
                    <input type="tel" name="telefono" id="telefono">
                </p>
                <!-- ///////////-->

                <!-- Campo Url -->
                <p>
                    <label for="url">Url:</label>
                    <input type="url" name="url" id="url">
                </p>
                <!-- ///////////-->
                
                <!-- Campo de seleccíon -->
                <p>
                    Campo de selección:
                    <select>
                        <option>Item # 1</option>
                        <option>Item # 2</option>
                        <option>Item # 3</option>
                    </select>
                </p>
                <!-- ///////////-->
                 
                <!-- Campo Radio -->
                <p>
                    <h4>Para seleccionar una opción</h4>
                    <label for="comida">Comida:</label> <br>
                    <input type="radio" name="comida">Hamburguesa
                    <input type="radio" name="comida">Ensalada
                    <input type="radio" name="comida">Papas fritas
                    <!-- deben tener el mismo name=" " Para que nos deje seleccionar uno de las opciones.-->
                </p>

                <!-- Campo checkbox o To do list -->
                <p>
                    <h4>Para seleccionar multiples opciones</h4>
                    <label for="comida">Comida:</label> <br>
                    <input type="checkbox" name="comida">Hamburguesa
                    <input type="checkbox" name="comida">Ensalada
                    <input type="checkbox" name="comida">Papas fritas
                    <!-- Estos input si pueden tener un name diferente -->
                </p>
                <!-- /////////////////////////////-->

                <!-- Campo de Color -->
                <p>
                    <label for="color">Color:</label>
                    <input type="color" name="color" id="color">
                </p>
                <!-- ///////////-->
            
                <!-- Campo área de texto -->
                <p>
                    <label for="txtarea">Comentarios:</label>
                    <textarea name="txtarea" id="txtarea" rows="8" cols="80"></textarea>
                    <!-- Si colocamos texto entre las etiquetas <textarea> Hola </textarea> este hola 
                         será como el atributo velue=" " y se verá en el campo de texto -->
                </p>
                <!-- ///////////-->
                
                <!-- Botón de enviar y reset -->
                <p>
                    <input type="submit" value="Enviar">
                    <input type="reset" value="Restablecer">
                </p>
                <!-- ///////////-->
           </fieldset>
           
           
           
           https://julianortiz6605.github.io/-4.5--Etiqueta-de-formulario/
