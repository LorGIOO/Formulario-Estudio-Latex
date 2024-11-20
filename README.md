# Proyecto de Formulario Académico

Este proyecto tiene como objetivo crear un formulario en formato PDF diseñado para facilitar el estudio de asignaturas que contienen una gran cantidad de fórmulas, proyectos o trabajos. La idea principal es estructurar de forma clara y accesible los contenidos esenciales de las materias, permitiendo a los estudiantes consultar fórmulas y definiciones de manera rápida y organizada.

Con la finalidad de facilitar el aprendizaje y la organización en asignaturas que requieren el uso de múltiples fórmulas o temas complejos. Es especialmente útil para estudiantes de ingeniería, física o cualquier disciplina técnica.
## Estructura del Proyecto

El PDF generado se compone de varias secciones, cada una destinada a organizar información clave. Los archivos `.tex` proporcionados constituyen los componentes individuales que se combinan para formar el documento completo. A continuación, se describen las secciones y los archivos involucrados:

### 1. **Portada**
   - Archivo: `Portada.tex`
   - Contiene la información de la portada, como el título del formulario, el nombre del autor y la asignatura.
   - Los logotipos utilizados son oficiales de la Universidad de La Laguna o cualquier otra organización educacional, los logos utilizados se pueden encontrar en la página oficial de la ULL: [Logotipos ULL](https://www.ull.es/portal/marca/logotipos/).

### 2. **Índice**
   - Archivo: `Indice.tex`
   - Presenta un índice completamente automatizado mediante la expresión `\sectionnc{}` o `\subsectionnc{}`que permite enlazar directamente con las secciones correspondientes del documento.

### 3. **Nomenclatura**
   - Archivo: `Nomenclatura.tex`
   - Define los símbolos, nombres y unidades que serán utilizados en las fórmulas. Cada fórmula está vinculada a este archivo, lo que permite redirigir al lector directamente a las definiciones y detalles de los símbolos al hacer `clic` sobre ellos.

### 4. **Temas y Contenidos**
   - Archivo: `Tema n.tex`
   - Este archivo y sus homólogos contiene las fórmulas de los temas especificados.

### 5. **Descripción**
   - Archivo: `Descripción.tex`
   - Proporciona una descripción detallada de las fórmulas, su uso práctico y contexto. Al hacer `Clic` en el nombre de una fórmula, el lector es redirigido a esta sección, donde se profundiza en su significado y aplicación.

### 6. **Archivo Principal**
   - Archivo: `Main_Formularios.tex`
   - Es la raíz de todos los archivos donde se insertaran las reglas o normas que deberá de cumplir el código, ya que es el nexo comun de todos los archivos donde se configura y se da forma al PDF final.

## Características Destacadas

- **Índice automatizado**: Permite navegar fácilmente por el contenido del formulario.
- **Enlaces interactivos**:
  - Los símbolos en las fórmulas redirigen al archivo `Nomenclatura.tex`, donde se detalla cada símbolo.
  - Los nombres de las fórmulas redirigen al archivo `Descripción.tex`, donde se proporciona información detallada sobre cada una.

## Requisitos de Software

Para trabajar con estos archivos de manera óptima, se recomienda utilizar un IDE adecuado junto con el lenguaje LaTeX. A continuación, se sugieren las siguientes herramientas:

- **IDE recomendado**: [TeXstudio](https://www.texstudio.org/)
- **Compilador LaTeX recomendado**: [MiKTeX](https://miktex.org/download)

### Configuración de TeXstudio

1. Descarga e instala TeXstudio y MiKTeX desde los enlaces anteriores.
2. Abre TeXstudio y accede a las opciones de configuración:
   - Ve a `Opciones > Configurar TeXstudio`.
   - En la pestaña `Vista previa`, busca el apartado `Orden`.
   - Cambia el compilador a `lualatex` o `xelatex`.
3. Esto asegurará que puedas visualizar correctamente el PDF generado con las configuraciones avanzadas utilizadas en este proyecto.
