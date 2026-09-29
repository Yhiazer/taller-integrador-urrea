# Taller integrador individual

**Nombre:** Benjamín Urrea Currihuinca
**Asignatura:** Buenas Prácticas de Desarrollo de Software

## Enlace a Netlify

https://taller-integrador-urrea.netlify.app/

## Descripción

Calculadora que recibe tres notas, calcula su promedio e indica si el resultado es aprobado (promedio igual o mayor a 3.0) o reprobado.

## Tabla de hallazgos

| Defecto encontrado | Por qué era un problema | Cómo lo corrigió |
|---|---|---|
| Archivo `Mi Pagina De Notas.HTML` | Tiene espacios y mayúsculas; los espacios complican las rutas y Netlify busca un `index.html` como página principal | Se renombró a `index.html` |
| Archivo `Estilos Del Sitio.CSS` | Tiene espacios y mayúsculas; no sigue la convención kebab-case para archivos | Se renombró a `style.css` y se actualizó el enlace en el HTML |
| Título de la pestaña `pagina` | No describe el contenido real de la página | Se cambió a `Calculadora de Promedio` |
| Variable `x` | No indica qué almacena, lo que obliga a leer todo el código para entenderla | Se renombró a `CANTIDAD_NOTAS`, siguiendo la convención de constantes |
| Variable `TempValue2` | El nombre no dice qué guarda y es poco descriptivo | Se renombró a `promedio` |
| Variables `a`, `b`, `c` | Letras sueltas que no indican que son notas | Se renombraron a `nota1`, `nota2` y `nota3` |
| Variable `data1` | Nombre genérico y además nunca se usaba | Se eliminó |
| Función `calc` | Nombre recortado que no indica bien qué función realiza | Se renombró a `calcularPromedio` |
| Identificadores `n1`, `n2`, `n3` | No indican qué campo representan dentro de la página | Se renombraron a `nota-1`, `nota-2` y `nota-3` |
| Identificadores `r` y `r2` | No indican qué información muestra cada párrafo | Se renombraron a `texto-promedio` y `texto-resultado` |
| Clase `cont1` | Nombre genérico que no indica qué contiene | Se renombró a `contenedor-general` |
| `console.log` de prueba | Mensajes de comprobación que no aportan nada, ya que la página funciona correctamente | Se eliminaron |
| Función `calcularAntiguo` comentada | Código sin uso que confunde y no aporta nada, ya que existe otra función que cumple esa tarea | Se eliminó |