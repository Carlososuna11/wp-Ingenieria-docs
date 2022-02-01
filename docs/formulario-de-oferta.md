# Formulario de Ofertas
****
## Descripción
_Este documento explica la configuración y utilización del formulario de ofertas_

## Modo de Acceso al Formulario:

1. En la página del administrador de Wordpress de su escuela, acceder a la sección de **Contacto** > **Formulario de Contacto**.
<p align="center"><img src="https://imgur.com/8jR7CaV.png"/></p> 

2. Seleccionar el formulario ya creado que aparece la lista de formularios. Este puede tener el nombre de `Ofertas` u `Ofertas - Caracas` (dependiendo de la escuela).


<p align="center"><img src="https://imgur.com/uPXfoQV.png"/></p> 

### Características del formulario:

Este formulario consta de 4 pestañas:

<p align="center"><img src="https://imgur.com/wot34Cr.png"/></p>

-  **Formulario**: Consiste en un editor de texto en donde se colocan los shortcodes de divi para cada campo del formulario. Para más información sobre los shortcodes y las funcionalidades de este formulario, consultar la [documentación](https://contactform7.com/editing-form-template/).

- **Correo**: En esta pestaña, se hacen las configuraciones de envío de correo electrónico. los campos que se muestran son:
    1. **Para**: En este campo se coloca el correo electrónico a quien se enviará el correo (EMcargado de las Prácticas Profesionales de cada escuela).
    2. **De**: En este campo se coloca el correo electrónico desde el que se enviará el correo. Por default es el correo de wordpress de la facultad. no es necesario cambiarlo.
    3. **Asunto**: En este campo se coloca el asunto del correo.
    4. **Cabeceras Adicionales**: Puede insertar campos de encabezado de mensaje adicionales aquí, como Cc y Bcc . Debe haber un campo por línea. 
    5. **Cuerpo del Mensaje**: En este campo se coloca el cuerpo del mensaje que se enviará.
    6. **Adjuntos**: En este campo se colocan los archivos que se adjuntarán al correo.

    Al correo se le pueden agregar shortcodes para colocar los datos del formulario. Por ejemplo, si se coloca el shortcode `[nombre]` en el campo de correo, se colocará el valor del campo de nombre. Para más información sobre los shortcodes, consultar la [documentación](https://contactform7.com/setting-up-mail/).

- **Mensajes**: En esta pestaña se configuraran todos los mensajes que el formulario mostrará, como lo son Mensajes de éxito, de error, de confirmación, etc. Para más información sobre los mensajes, consultar la [documentación](https://contactform7.com/editing-messages/).

- **Ajustes Adicionales**: Puede incluir configuraciones adicionales para cada formulario de contacto agregando fragmentos de código en el formato específico en el panel de la pestaña Configuración adicional en la pantalla del editor de formularios de contacto. Casos como solo permitir el uso de formularios a los suscritos, modo demostración, código Javascript, etc. Para más información sobre los ajustes adicionales, consultar la [documentación](https://contactform7.com/additional-settings/).

## Configuración del formulario de Ofertas

### **Pestaña de Formulario**
En esta pestaña estan los shortcodes de divi para cada campo del formulario. Cabe destacar que este complemento de divi genera un formulario sin diseño alguno, y es por ello que, además de los shortcodes, estan inscrustados etiquetas `HTML` con clases `CSS` para poder usar el tema de formulario de la facultad.

<p align="center"><img src="https://imgur.com/8mTFGG9.png"/></p>

#### Los campos del formulario son:
 
- **Nombre de la Oferta**: Este campo es obligatorio.
- **Nombre de la Empresa**: Este campo es obligatorio.
- **Sitio Web de la Empresa**: Este campo es obligatorio.
- **Nombre del Autor de la Oferta**: Este campo es obligatorio.
- **Número de teléfono del Autor de la Oferta**: Este campo es obligatorio.
- **Correo electrónico del Autor de la Oferta**: Este campo es obligatorio.
- **Descripción de la Oferta**: Este campo es obligatorio.
- **Url de la Imagen Destacada de la Oferta**: Este campo es obligatorio.
- **Modalidad del Contrato**: Este campo es obligatorio.
- **Tipo de Contrato**: Este campo es obligatorio.
- **Requisitos del Cargo**: Este campo es obligatorio.

### Pestaña de Correo

En esta vista se configuró los shortcodes anteriores en el cuerpo del mensaje. A continuación se muestra un ejemplo del mismo

```
De: [nombre] 
Asunto: [post-title]

Nombre de la oferta:
[post-title]

Nombre de la empresa:
[nombre_de_la_empresa]

Sitio web:
[sitio_web]

Nombre del Contacto:
[nombre]

Numero de teléfono:
[numero_de_telefono]

Correo electrónico:
[correo_electronico]

Descripción del cargo:
[descripcion_del_cargo]

Imagen destacada:
<img src="[your-file]" style="border-style:solid" /> 

Modalidad del contrato:
[modalidad_de_contrato]

Tipo de Oferta:
[tipo]

Requisitos del cargo:
[requisitos]





Luego de comprobar esta información y ponerse en contacto con la empresa en cuestión, si se desea publicar la oferta en la página web, deberá cargar la información del presente correo en el pod de ofertas.

-- 
Este mensaje se ha enviado desde un formulario de contacto en [_site_title] ([_site_url])
```

El correo al cual llegará la oferta, es al del encargado de las prácticas profesionales de cada escuela.


## Como cargar la oferta en la página:

1. Una vez recibido el correo con la oferta, el encargado de las prácticas profesionales de cada escuela deberá ponerse en contacto con el empleador de la misma, con la finalidad de aclarar detalles y finalizar el acuerdo.
2. Ya con toda la información de la oferta en mano, en la página del administrador de Wordpress de su escuela, acceder a la sección de **Ofertas** > **Agregar una oferta**.
<p align="center"><img src="https://i.imgur.com/VznG9pP.png"/></p> 
3. Lo primero que se agregará será el título de la oferta.
<p align="center"><img src="https://i.imgur.com/WSpx5u5.jpeg"/></p> 
4. Seguido de ello, se procederá a ingresar la información que se recibió en el correo, en los campos a los cuales corresponda cada información, los cuales se encuentra al final de la página.
<p align="center"><img src="https://i.imgur.com/QSqQZdz.jpeg"/></p> 
5. Luego, a mano derecha, se agregará la imagen destacada de la oferta. Para ello primero se deberá subir la imagen a la biblioteca, para luego poder seleccionarla.
<p align="center"><img src="https://i.imgur.com/QSqQZdz.jpeg"/></p> 
6. Después, solo quedará seleccionar también a mano derecha, el modo de contrato y el tipo de la oferta (se agrega tanto en el paso 3 como en este), ya que si no se seleccionan los campos aquí, el pod no funcionará correctamente.
<p align="center"><img src="https://i.imgur.com/4CcE47Y.jpeg"/></p> 
7. Ya para finalizar, solo queda verificar una vez más que todos los datos e información que se hayan cargado sean los correctos, y de ser así, se publicará la oferta.
<p align="center"><img src="https://i.imgur.com/8zzOtw4.jpeg"/></p> 

Se recomienda que una vez publicada la oferta, se compruebe que la misma se visualice sin problemas en la página de de ofertas de la escuela.



## Como colocar el formulario en una página:

1. Copiar el shortcode `[contact-form-7 id="__ID_FORMULARIO__" title="__TITULO_FORMULARIO__"]` en la página donde desea colocar el formulario. Utilice un componente de código o de texto de los que provee DIVI. Para más información, consultar en la [documentación](https://www.elegantthemes.com/documentation/divi/code/) de DIVI.

**Pista**: El id del formulario y el titulo aparecen en la vista de configuración del formulario. y en la Lista de formularios de contacto.

<p align="center"><img src="https://imgur.com/pDYmyOR.png"/></p>
