# AboutMe

Este proyecto trata de crear un AboutMe personal donde he trabajado todos los aspectos de una página web.
## Configuración:

Configurar primeramente los archivos lib/mixins.scss y lib/variables.scss

Es recomendable configurar dichos archivos para los distintos tamaños, colores, espacios...

Nomenclatura:
La convención de nombre sigue este patrón:

    .bloque{}
    .bloque__elemento{}
    .bloque--modificador{}
'.bloque' representa el primer nivel de una abstracción o componente.
'.bloque__elemento' representa un descendente de '.bloque' que se ayuda de '.bloque' como un conjunto.
'.bloque--modificador' representa un estado diferente de '.bloque'.
    .habitacion{}
    .habitacion--cocina{}
        .habitacion--cocina__nevera{}
        .habitacion--cocina__nevera .nevera--congelador{__}
        .habitacion--cocina__nevera .nevera--congelador__primera-altura{}
        .habitacion--cocina__nevera .nevera--congelador__segunda-altura{}
        .habitacion--cocina__nevera .nevera--congelador__tercera-altura{}
Organización
Lor archivos de SCSS están todos en el archivo scss/style.scss con una distribución explicada de la siguiente manera:

--scss
    style.scss

        /*------------------------------------*\
        $SETTINGS
        \*------------------------------------*/
            settings/mixings.scss
            settings/variables.scss

        /*------------------------------------*\
            $UTILITIES
        \*------------------------------------*/
            utilities.scss
            flex.scss

        
        /*------------------------------------*\
            $COMPONENTS
        \*------------------------------------*/
            navbar.scss
            perfil.scss
            gridcells.scss
            buttons.scss
            forms.scss
            formulario.scss


        /*------------------------------------*\
            $LAYOUT
        \*------------------------------------*/
            header.scss
            skills.scss
            aficiones.scss
            footer.scss


El archivo style.css nos indica donde tenemos nuestros elementos y su nombre, gracias a los comentarios BEM na búsqueda cmd/ctrl + f en nuestro editor que empiece por $NOMBREDESECCION nos ayudará mucho a encontrar el contenido.

A su vez están todas las secciones separadas unas de las otras para ubicar rápidamente cuando echamos un vistazo.

Instalación
Necesitarás obligatoriamente tener un preprocesador instalado.
