# Registro Moderno

Este proyecto implementa un formulario de registro moderno, desarrollado con HTML, CSS y JavaScript puro.  
El objetivo es ofrecer una interfaz limpia, validaciones dinámicas y una experiencia de usuario fluida y profesional.

---

## Descripción general

El formulario permite registrar datos básicos de un usuario, realizando validaciones en tiempo real antes de aceptar el envío.  
Incluye manejo visual de errores, confirmación de contraseñas y verificación de aceptación de términos y condiciones.

---

## Características principales

- Diseño moderno con sombras suaves y bordes redondeados.  
- Validaciones en tiempo real con mensajes de error específicos.  
- Sistema de alertas visuales para mostrar éxito o error en el registro.  
- Campos adicionales para fecha de nacimiento y género.  
- Interfaz completamente responsiva.  
- Paleta de colores personalizable mediante variables CSS.  

---

## Tecnologías utilizadas

| Tecnología | Descripción |
|-------------|--------------|
| **HTML5** | Define la estructura principal del formulario y sus campos. |
| **CSS3** | Estiliza el formulario con un diseño moderno, colores vibrantes y efectos visuales. |
| **JavaScript (Vanilla)** | Gestiona la validación de campos, manejo de errores y retroalimentación visual. |

---

## Estructura del proyecto

formulario/
│
├── index.html # Contiene la estructura principal, estilos y script integrados
├── README.md # Documentación del proyecto

---

## Campos del formulario

| Campo | Tipo | Descripción |
|--------|------|-------------|
| Nombre completo | Texto | Requiere al menos 3 caracteres. |
| Correo electrónico | Email | Debe cumplir el formato de correo válido. |
| Contraseña | Password | Mínimo 8 caracteres. |
| Confirmar contraseña | Password | Debe coincidir con la contraseña anterior. |
| Fecha de nacimiento | Date | Campo opcional. |
| Género | Select | Masculino, femenino u otro. |
| Términos y condiciones | Checkbox | Debe estar marcado para continuar. |

---

## Validaciones implementadas

| Validación | Condición | Mensaje mostrado |
|-------------|------------|------------------|
| Nombre | Menos de 3 caracteres | “El nombre debe tener al menos 3 caracteres.” |
| Email | Formato inválido | “Ingresa un correo válido.” |
| Contraseña | Menos de 8 caracteres | “La contraseña debe tener mínimo 8 caracteres.” |
| Confirmar contraseña | No coincide con la anterior | “Las contraseñas no coinciden.” |
| Términos | Casilla no marcada | “Debes aceptar los términos.” |

Cuando todas las validaciones se cumplen, se muestra un mensaje de éxito:  
**“Registro completado correctamente.”**

Si hay errores, aparece el mensaje:  
**“Revisa los campos con errores.”**

---

## Paleta de colores

| Variable | Descripción | Código |
|-----------|--------------|--------|
| `--bg` | Fondo general | `#f0f4f8` |
| `--card-bg` | Fondo de la tarjeta | `#ffffff` |
| `--primary` | Color principal (morado) | `#6c5ce7` |
| `--accent` | Color acento (verde aqua) | `#00b894` |
| `--error` | Color de error | `#d63031` |
| `--success` | Color de éxito | `#00b894` |
| `--btn-hover` | Color del botón al pasar el cursor | `#341f97` |

Estas variables se pueden modificar desde el bloque `:root` del archivo CSS para adaptar la apariencia del formulario.

---

## Cómo ejecutar el proyecto

1. Clona el repositorio:
   ```bash
   git clone https://github.com/DennisP10/formulario.git
2.Abre el archivo index.html en tu navegador.
3.Interactúa con el formulario y verifica el funcionamiento de las validaciones.

Personalización

Puedes agregar nuevos campos siguiendo la misma estructura de validación.

Es posible separar el CSS y el JavaScript en archivos independientes (style.css, script.js) para mejorar la organización.

Si deseas conectarlo con una base de datos o backend, puedes integrar APIs REST, Firebase, Node.js o PHP.

Autor

Dennis Pérez
Repositorio: github.com/DennisP10/formulario
