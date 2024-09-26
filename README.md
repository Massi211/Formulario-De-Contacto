# Formulario de Contacto

Este es un formulario de contacto básico que utiliza [FormSubmit](https://formsubmit.co) para enviar las consultas de los usuarios por correo electrónico. A continuación, se detallan los campos del formulario y las instrucciones para su uso.

## Descripción

El formulario permite a los usuarios enviar una consulta ingresando su nombre, correo electrónico y mensaje. Los datos se enviarán a la dirección de correo electrónico especificada a través del servicio FormSubmit.

## Campos del formulario

- **Nombre:** Campo de texto donde el usuario debe ingresar su nombre.
- **Correo:** Campo de entrada para que el usuario ingrese su correo electrónico. Se valida automáticamente para asegurarse de que se trata de un correo válido.
- **Consulta:** Área de texto donde el usuario escribe su consulta o mensaje.
- **Condiciones:** Casilla de verificación que el usuario debe marcar para aceptar las condiciones antes de enviar el formulario.

## Estructura del formulario

El formulario está compuesto por las siguientes etiquetas:

- `<form>`: Utiliza el método `POST` para enviar los datos al servicio de FormSubmit.
- `<input type="text">`: Campo para ingresar el nombre del usuario.
- `<input type="email">`: Campo para ingresar el correo electrónico.
- `<textarea>`: Área de texto para la consulta del usuario.
- `<input type="checkbox">`: Casilla para aceptar los términos y condiciones. Es un campo obligatorio.
- `<button>`: Botón para enviar el formulario.

## Configuración

El formulario está configurado para enviar los datos a la dirección de correo electrónico `""`. Si deseas cambiar la dirección de correo electrónico de destino, simplemente modifica la URL en el atributo `action` del formulario:

```html
<form action="https://formsubmit.co/tu-correo@ejemplo.com" method="post">
