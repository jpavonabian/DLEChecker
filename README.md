# DLEChecker

## Buscador de definiciones en el Diccionario de la Lengua Española.

### Introducción.

El complemento DLEChecker para NVDA permite a los usuarios consultar de forma rápida y accesible cualquier definición de una palabra en el [Diccionario de la Lengua Española de la RAE](https://dle.rae.es/) (Real Academia Española).

Este es  el máximo órgano consultivo en cuanto a la ortografía y la gramática de la misma, el cual se encarga de garantizar una norma común, así como de velar que los cambios que esta experimente no quiebren la esencial unidad que mantiene en todo el ámbito hispánico.

Así mismo, también es posible conocer   los sinónimos y antónimos del término buscado, gracias al diccionario de sinónimos de Wordreference.

### Modo de uso.

Este complemento dispone de dos modos de utilización, explicados a continuación:

a) El modo tradicional hasta el momento en DLEChecker. Es decir, seleccionando cualquier palabra (utilizando shift+teclas habituales de navegación por texto), y pulsando la combinación de teclas NVDA + Shift + C.

b) Pulsando directamente la combinación de teclas NVDA + Shift + C en cualquier aplicación.

En el primer caso, DLEChecker mostrará la definición del término buscado así como los sinónimos y/o antónimos disponibles en la ventana de resultados existente en la versión 1.1.

En el segundo caso, DLEChecker mostrará un cuadro de diálogo donde introducir el término a buscar. Una vez introducido y presionado el botón "Consultar", el complemento mostrará la ventana de resultados habitual.

Se pueden utilizar las flechas para navegar por el contenido de la ventana de resultados, o bien hacer que NVDA lo lea automáticamente y lo copie al portapapeles empleando los botones dispuestos a tal efecto en el diálogo.

Si se seleccionan accidentalmente varias palabras y se ejecuta la búsqueda, el complemento sólo tendrá en cuenta la primera.

La combinación de teclas NVDA + Shift + C puede ser personalizada a través del cuadro de diálogo «Gestos de Entrada» de la opción «Preferencias» de NVDA dentro de la categoría DLEChecker.

### Atajos.

El único atajo disponible por el momento en este complemento, es la combinación de teclas NVDA + Shift + C. Es el encargado de mostrar el cuadro de diálogo de entrada para introducir el término a buscar, así como de realizar la consulta a la web del Diccionario de la Lengua Española de la RAE.

## Registro de cambios.

### Versión 2.1.

* Modificado el algoritmo principal de DLEChecker para la consulta de términos debido a la modificación de la estructura de la web del Diccionario de la Lengua Española de la RAE. Gracias a Jesús Pavón, @jpavonabian@mst.universoalterno.es, por el Pull Request que ha permitido la actualización del complemento.
* Corregido un error que impedía desde la versión anterior, la búsqueda de un nuevo término, sin necesidad de su selección previa.

### Versión 2.0.

* Reestructurado el código del complemento para mejorar la obtención de todas las acepciones del término introducido, así como la obtención de los sinónimos y antónimos de cada acepción desde la web de la Real Academia Española.
* Eliminada la consulta externa a wordreference.com a fin de obtener los sinónimos y antónimos.
* Modificado el archivo README.md a fin de reflejar el cambio de versión y las últimas correcciones realizadas.

### Versión 1.3.2.3.

* Actualizada la compatibilidad de DLEChecker con NVDA 2023.1.0.
* Modificado el archivo README para dejar constancia de un cambio producido en la versión 1.3.2 faltante.
* Modificado el complemento para que ponga la palabra buscada en minúsculas incluso en el cuadro de búsqueda, para evitar posibles errores. Gracias a Sukil Echenique por su contribución.
* Quitado el BOM (Byte Order Mark o Marca de Orden de Bytes) de la ayuda del complemento, para evitar problemas de codificación. Gracias a Sukil Echenique por su contribución.
* Añadido un párrafo en la ayuda del complemento que aclara que los sinónimos y antónimos se buscan en wordreference. Gracias a Sukil Echenique por su contribución.
* Corregido un error que ignoraba los guiones del término de búsqueda. Ahora DLEChecker permite buscar prefijos y sufijos. Gracias a Sukil Echenique por su contribución.

### Versión 1.3.2.2.

* Actualizada la compatibilidad de DLEChecker con NVDA 2022.1.

### Versión 1.3.2.1.

* Corregido un error que impedía que se cargasen todos los módulos necesarios para el correcto funcionamiento de DLEChecker al eliminar antes de tiempo la ruta del complemento del path de NVDA.

### Versión  1.3.2.

* Modificado un error en el path de NVDA. Quitada la referencia de la ruta del complemento del mismo, a fin de evitar posibles problemas en el futuro.
* Modificado un error que impedía que se mostrasen las definiciones cuando el término era  una locución. Gracias a Sukil Echenique por su contribución.
* Corregido el título y el estilo de los diálogos de error. Gracias a Sukil Echenique por su contribución.

### Versión 1.3.1.

* Actualizada la compatibilidad de DLEChecker con NVDA 2021.1.

### Versión 1.3.

* Modificada la función principal del complemento para que muestre todas las definiciones del término buscado, aunque éste tenga varias acepciones. Gracias a Peter Reina, Georgiana Frincu y Marta Estrada por reportar el error.
* Corregido un error que hacía que al intentar recuperar los sinónimos y antónimos de un término buscado, lanzase una excepción, indicando que no habían pese a que sí existían. Gracias a Marta Estrada por reportarlo.
* Modificada la visualización del resultado para que estéticamente quede mejor formateado.

### Versión 1.2.3.

* Solucionado un error que impedía buscar las definiciones de términos que incluyesen el carácter 'ü' entre sus letras.

### Versión 1.2.2.

* Solucionado un error que impedía el correcto funcionamiento de DLEChecker cuando existían complementos instalados que importaban el módulo "html", interfiriendo con el importado por él.

### Versión 1.2.1.

* Corregido un error que hacía que con conexiones lentas NVDA quedase bloqueado mientras realizaba la consulta, impidiendo el normal funcionamiento del mismo.

### Versión 1.2.

* Añadida una nueva característica que permite obtener los sinónimos y antónimos del término buscado a la vez que la definición. Agradecer a Jose Manuel Delicado por su ayuda implementando esta función.
* Modificada la interfaz visual ligeramente para una mejor visualización y coherencia con el complemento. Agradecer a Héctor Benítez por sus sugerencias en este sentido.
* Corrección de errores y mejoras de estabilidad.

### Versión 1.1.

* Corrección de un error que hacía fallar el complemento al intentar obtener la definición de una palabra en mayúsculas.
* Sustitución del cuadro de diálogo de NVDA donde se mostraba la definición de la palabra por una interfaz gráfica más amigable, donde se han añadido también las opciones "Leer resultado", "Copiar al portapapeles" y "Salir". Puede navegarse a estas opciones pulsando tabulador desde el cuadro de edición. Agradecer a Héctor Benítez @HXeBoLaX su contribución.

### Versión 1.0.

* Versión inicial.
