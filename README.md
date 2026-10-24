# EZScript

EZScript es un lenguaje de programacion diseñado para ser colorido facil y divertido de usar

## Formatos

Los formatos se dividen en 2 partes:

- **.ez**: El formato EZScript tradicional, el archivo seco

- **.ezp**: El formato empaquetado de archivos EZScript y significa ***EZScript Package***

## Versiones

Las versiones tambien se dividen en 2 partes

-**EZScript (Python con Tkinker)**: es la version normal de EZScript

-**EZScript HTML (Web)**: a diferencia de EZScript normal esta version es la version web diseñado para NO tener que instalar Python 

-**EZScripting**: El motor de EZScript

## Capturas de pantalla

| EZScript (Python) | EZScript HTML |
| :-- | --:
| <img width="1919" height="1031" alt="Captura de pantalla 2026-10-13 123719" src="https://github.com/user-attachments/assets/f73d1753-c634-45a3-a117-68e1fd3f0bbb"> | <img width="1917" height="942" alt="Captura de pantalla 2026-10-13 123833" src="https://github.com/user-attachments/assets/fcac18e1-b03d-4a5f-8e5c-56c1969169c9" /> |

##  Comandos

Referencia completa de los **~250 comandos** de EasyScript, agrupados por categoría. Todos funcionan en **ES / EN / PT** — por ejemplo `mostrar` = `show` = `exibir`.

###  Salida

| Comando | Descripción |
|---------|-------------|
| `mostrar "texto"` | Imprime un texto o valor en la consola. |
| `print "texto"` | Alias de `mostrar`. |
| `limpiar_pantalla` | Borra la consola **y** el canvas. |
| `limpiar_consola` | Borra solo la consola. |
| `boton:("texto", accion)` | Crea un botón interactivo en la consola que ejecuta `accion` al pulsarlo. |

###  Variables y entrada

| Comando | Descripción |
|---------|-------------|
| `var:(nombre, valor)` | Declara o asigna una variable. |
| `incrementar:(var, n)` | Suma `n` al valor de la variable (si no se da `n`, suma 1). |
| `decrementar:(var, n)` | Resta `n` al valor de la variable (si no se da `n`, resta 1). |
| `asignar:(var, valor)` | Asigna un valor a una variable existente. |
| `entrada:(var, "mensaje")` | Pide al usuario un valor por diálogo. |

###  Cadenas de texto

| Comando | Descripción |
|---------|-------------|
| `mayusculas:(var)` | Convierte el texto de la variable a MAYÚSCULAS. |
| `minusculas:(var)` | Convierte el texto de la variable a minúsculas. |
| `longitud:(expr)` | Muestra en consola la longitud de un texto. |
| `reemplazar:(var, viejo, nuevo)` | Sustituye todas las apariciones de `viejo` por `nuevo`. |
| `concatenar:(var, a, b)` | Une `a + b` en la variable. |
| `dividir_texto:(var, txt, sep)` | Divide un texto por un separador → lista. |
| `indice:(var, lista, i)` | Obtiene el elemento en la posición `i`. |
| `invertir:(var, txt)` | Invierte el orden de los caracteres. |
| `unir:(var, a, b)` | Alias de `concatenar`. |
| `trim:(var, txt)` | Quita espacios al principio y al final. |
| `trim_izq:(var, txt)` | Quita espacios solo al principio. |
| `trim_der:(var, txt)` | Quita espacios solo al final. |
| `subcadena:(var, txt, ini, fin)` | Extrae el texto entre las posiciones `ini` y `fin`. |
| `empieza_con:(var, txt, prefijo)` | `true` si `txt` empieza con `prefijo`. |
| `termina_con:(var, txt, sufijo)` | `true` si `txt` termina con `sufijo`. |
| `buscar_pos:(var, txt, busq)` | Devuelve la posición de `busq` dentro de `txt`, o -1. |
| `capitalizar:(var, txt)` | Pone la primera letra mayúscula y el resto minúsculas. |
| `repetir_texto:(var, txt, n)` | Repite el texto `n` veces. |
| `formato:(var, plantilla, valores)` | Rellena `{0}`, `{1}`… con los valores dados. |

###  Conversión de tipos

| Comando | Descripción |
|---------|-------------|
| `tipo_dato:(expr)` | Muestra el tipo de dato en consola. |
| `a_numero:(var, valor)` | Convierte un valor a número. |
| `a_texto:(var, valor)` | Convierte un valor a texto. |
| `a_lista:(var, valor)` | Convierte un valor iterable a lista. |

###  Matemáticas básicas

| Comando | Descripción |
|---------|-------------|
| `sumar:(var, a, b)` | `var = a + b`. |
| `restar:(var, a, b)` | `var = a - b`. |
| `multiplicar:(var, a, b)` | `var = a * b`. |
| `dividir:(var, a, b)` | `var = a / b`. |
| `modulo:(var, a, b)` | `var = a % b` (resto). |
| `potencia:(var, a, b)` | `var = a ^ b`. |
| `raiz:(var, x)` | Raíz cuadrada. |
| `absoluto:(var, x)` | Valor absoluto. |
| `redondear:(var, x)` | Redondea al entero más cercano. |
| `piso:(var, x)` | Redondea hacia abajo. |
| `techo:(var, x)` | Redondea hacia arriba. |
| `truncar:(var, x)` | Elimina la parte decimal. |
| `signo:(var, x)` | Devuelve -1, 0 o 1. |
| `maximo:(var, a, b)` | El mayor de dos números. |
| `minimo:(var, a, b)` | El menor de dos números. |
| `pi:(var)` | Guarda el valor de π (3.14159…). |

###  Matemáticas avanzadas

| Comando | Descripción |
|---------|-------------|
| `seno:(var, x)` | Seno (x en grados). |
| `coseno:(var, x)` | Coseno (x en grados). |
| `tangente:(var, x)` | Tangente (x en grados). |
| `arcoseno:(var, x)` | Arcoseno (resultado en grados). |
| `arcocoseno:(var, x)` | Arcocoseno (resultado en grados). |
| `arcotangente:(var, x)` | Arcotangente (resultado en grados). |
| `log_natural:(var, x)` | Logaritmo natural (base e). |
| `log_base10:(var, x)` | Logaritmo en base 10. |
| `log_base:(var, base, x)` | Logaritmo en base arbitraria. |
| `exponencial:(var, x)` | e^x. |
| `factorial:(var, n)` | n! (factorial). |
| `gcd:(var, a, b)` | Máximo común divisor. |
| `lcm:(var, a, b)` | Mínimo común múltiplo. |

###  Aleatoriedad

| Comando | Descripción |
|---------|-------------|
| `semilla:(n)` | Fija la semilla para reproducibilidad. |
| `random:(var, min, max)` | Número entero aleatorio en `[min, max]`. |
| `random_flotante:(var, min, max)` | Número decimal aleatorio. |
| `elegir:(var, lista)` | Elige un elemento al azar de la lista. |
| `barajar:(var, lista)` | Devuelve la lista mezclada. |
| `muestra:(var, lista, n)` | Extrae `n` elementos al azar sin repetir. |

###  Lógica

| Comando | Descripción |
|---------|-------------|
| `igual_a:(var, a, b)` | `true` si `a` es igual a `b`. |
| `mayor_que:(var, a, b)` | `true` si `a > b`. |
| `menor_que:(var, a, b)` | `true` si `a < b`. |
| `y:(var, a, b)` | AND lógico. |
| `o:(var, a, b)` | OR lógico. |
| `no:(var, a)` | NOT lógico. |

###  Bits

| Comando | Descripción |
|---------|-------------|
| `bit_and:(var, a, b)` | AND a nivel de bits. |
| `bit_or:(var, a, b)` | OR a nivel de bits. |
| `bit_xor:(var, a, b)` | XOR a nivel de bits. |
| `bit_not:(var, a)` | NOT a nivel de bits. |
| `shl:(var, a, n)` | Desplaza `a` `n` bits a la izquierda. |
| `shr:(var, a, n)` | Desplaza `a` `n` bits a la derecha. |

###  Listas

| Comando | Descripción |
|---------|-------------|
| `lista:(var)` | Crea una lista vacía. |
| `agregar:(var, x)` | Añade un elemento al final. |
| `quitar:(var, x)` | Elimina la primera aparición de `x`. |
| `obtener:(var, lista, i)` | Devuelve el elemento en la posición `i`. |
| `ordenar:(var, lista)` | Ordena de menor a mayor. |
| `contar:(expr)` | Muestra la longitud de una lista o texto. |
| `longitud_lista:(var, lista)` | Guarda la longitud en una variable. |
| `suma_lista:(var, lista)` | Suma todos los elementos numéricos. |
| `max_lista:(var, lista)` | Valor máximo. |
| `min_lista:(var, lista)` | Valor mínimo. |
| `promedio_lista:(var, lista)` | Media aritmética. |
| `unir_lista:(var, sep, lista)` | Une con un separador → texto. |
| `filtro_pares:(var, lista)` | Devuelve solo los números pares. |
| `filtro_impares:(var, lista)` | Devuelve solo los números impares. |
| `mapear_doble:(var, lista)` | Multiplica cada elemento por 2. |
| `indice_lista:(var, lista, x)` | Índice de `x` en la lista. |
| `contar_valor:(var, lista, x)` | Cuántas veces aparece `x`. |
| `aplanar:(var, lista)` | Aplana listas anidadas un nivel. |
| `unico:(var, lista)` | Elimina duplicados manteniendo orden. |
| `zip_lista:(var, a, b)` | Combina dos listas en pares. |
| `rango:(var, ini, fin)` | Lista de números enteros `[ini, fin)`. |
| `eliminar_duplicados:(var, lista)` | Elimina duplicados (equivalente a `unico`). |
| `contiene:(var, lista, x)` | `true` si la lista contiene `x`. |

###  Control de flujo

| Comando | Descripción |
|---------|-------------|
| `si:(cond)` … `fin_si` | Bloque condicional. |
| `sino:` | Bloque alternativo. |
| `mientras:(cond)` … `fin_mientras` | Bucle mientras la condición sea cierta. |
| `bucle:(n)` … `fin_bucle` | Repite `n` veces. |
| `romper` | Sale del bucle inmediatamente. |
| `continuar` | Salta a la siguiente iteración. |
| `detener` | Detiene la ejecución del script. |

###  Funciones

| Comando | Descripción |
|---------|-------------|
| `funcion:(nombre, args...)` … `fin_funcion` | Define una función. |
| `llamar:(nombre, args...)` | Llama a una función. |
| `retornar:(valor)` | Devuelve un valor y sale de la función. |

###  Clases y objetos

| Comando | Descripción |
|---------|-------------|
| `clase:(Nombre[, Padre])` … `fin_clase` | Define una clase (con herencia opcional). |
| `propiedad:(nombre, valor)` | Define un campo dentro de la clase. |
| `nuevo:(var, Clase)` | Instancia un objeto. |
| `llamar_metodo:(obj, metodo, args...)` | Llama a un método de un objeto. |
| `hereda:(Clase, Padre)` | Declara herencia (alternativa). |

###  Tests

| Comando | Descripción |
|---------|-------------|
| `test:("nombre")` … `fin_test` | Bloque de test. |
| `afirmar_igual:(a, b)` | Falla si `a != b`. |
| `afirmar_verdad:(x)` | Falla si `x` es falso. |
| `afirmar_falso:(x)` | Falla si `x` es verdadero. |

###  Eventos y timers

| Comando | Descripción |
|---------|-------------|
| `al:("evento", funcion)` | Registra un handler para un evento. |
| `emitir:("evento")` | Dispara un evento (llama a sus handlers). |
| `cada:(id, ms, funcion)` | Ejecuta `funcion` cada `ms` milisegundos. |
| `cancelar_timer:(id)` | Cancela un timer. |
| `tecla_al:("tecla", evento, funcion)` | Asocia una tecla a una función (canvas). |
| `raton_al:("click"\|"move", funcion)` | Asocia un evento de ratón a una función. |
| `animar:(sprite, dx, dy, pasos, delay)` | Anima un sprite (uso avanzado). |

###  Sprites y juegos

| Comando | Descripción |
|---------|-------------|
| `sprite:(nombre, x, y, w, h, color)` | Crea un sprite. |
| `mover_sprite:(nombre, dx, dy)` | Mueve un sprite relativamente. |
| `dibujar_sprite:(nombre)` | Redibuja un sprite. |
| `colisiona:(var, s1, s2)` | `true` si dos sprites se solapan. |
| `gravedad:(sprite, g)` | Aplica gravedad (uso avanzado). |

###  Dibujo en canvas

| Comando | Descripción |
|---------|-------------|
| `color:("rojo")` | Fija el color de dibujo actual. |
| `color_canvas:("azul")` | Alias de `color`. |
| `rgb:(r, g, b)` | Fija el color con valores RGB. |
| `grosor_linea:(n)` | Ancho de las líneas en píxeles. |
| `linea:(x1, y1, x2, y2[, color])` | Dibuja una línea. |
| `rectangulo:(x, y, w, h[, color])` | Dibuja un rectángulo relleno. |
| `circulo:(x, y, r[, color])` | Dibuja un círculo relleno. |
| `ovalo:(x, y, w, h[, color])` | Dibuja una elipse rellena. |
| `triangulo:(x1,y1,x2,y2,x3,y3[,color])` | Dibuja un triángulo. |
| `texto_canvas:(x, y, "txt"[, color])` | Escribe texto en el canvas. |
| `cuadricula:(paso)` | Dibuja una cuadrícula de fondo. |
| `pixel:(x, y[, color])` | Pinta un píxel. |
| `borrar_canvas` | Borra todo el canvas. |

###  Modos gráficos

| Comando | Descripción |
|---------|-------------|
| `modo_grafico:("normal"\|"8bit"\|"16bit")` | Cambia el modo gráfico (retematiza el IDE). |
| `paleta:("nes"\|"gameboy"\|"cga"\|"snes"\|"vga"\|"sinclair")` | Cambia la paleta retro. |
| `idioma:("es"\|"en"\|"pt")` | Cambia el idioma del IDE en caliente. |

###  Audio

| Comando | Descripción |
|---------|-------------|
| `nota:(frecuencia, ms)` | Reproduce una frecuencia durante `ms` milisegundos. |
| `beep:(frecuencia, ms)` | Alias de `nota`. |
| `pitido` | Beep corto por defecto. |
| `musica:("do,re,mi,fa")` | Reproduce una secuencia de notas. |

###  Fecha y hora

| Comando | Descripción |
|---------|-------------|
| `fecha` | Imprime la fecha actual (YYYY-MM-DD). |
| `hora` | Imprime la hora actual (HH:MM:SS). |
| `hora_actual` | Alias de `hora`. |
| `fecha_hora` | Imprime fecha + hora. |
| `año:(var)` | Guarda el año actual. |
| `mes:(var)` | Guarda el mes actual. |
| `dia:(var)` | Guarda el día actual. |
| `hora_num:(var)` | Guarda la hora (0-23). |
| `minuto:(var)` | Guarda el minuto. |
| `segundo:(var)` | Guarda el segundo. |
| `timestamp:(var)` | Guarda el timestamp Unix. |
| `formatear_fecha:(var, "%Y-%m-%d")` | Formatea la fecha actual con `strftime`. |
| `esperar:(segundos)` | Pausa la ejecución. |

###  Diálogos y sistema

| Comando | Descripción |
|---------|-------------|
| `alerta:("msg")` | Muestra un diálogo con el mensaje. |
| `confirmar:(var, "pregunta")` | Diálogo Sí/No → `true`/`false`. |
| `abrir_url:("https://...")` | Abre una URL en el navegador. |
| `copiar:("texto")` | Copia al portapapeles. |
| `notificacion:("título"[, "cuerpo"])` | Muestra una notificación. |
| `sistema:(var)` | Guarda el nombre del SO. |
| `arquitectura:(var)` | Arquitectura (x86_64, arm64…). |
| `usuario:(var)` | Nombre del usuario actual. |
| `cwd:(var)` | Directorio de trabajo actual. |
| `variable_entorno:(var, "HOME")` | Lee una variable de entorno. |
| `proceso_id:(var)` | Guarda el PID del proceso. |

###  Shell (solo Python)

| Comando | Descripción |
|---------|-------------|
| `ejecutar_shell:(var, "cmd")` | Ejecuta un comando de shell y captura la salida. |
| `ejecutar_cmd:(var, "prog args")` | Igual pero sin shell intermedio. |

> ⚠️ No disponible en la versión HTML (navegador).

###  Archivos (VFS)

| Comando | Descripción |
|---------|-------------|
| `crear_archivo:(ruta, contenido)` | Crea o sobrescribe un archivo. |
| `leer_archivo:(var, ruta)` | Lee el contenido completo. |
| `existe_archivo:(var, ruta)` | `true` si el archivo existe. |
| `eliminar_archivo:(ruta)` | Borra un archivo. |
| `listar_archivos:(var[, ruta])` | Lista los archivos (VFS o carpeta). |
| `copiar_archivo:(src, dst)` | Copia un archivo. |
| `mover_archivo:(src, dst)` | Mueve un archivo. |
| `renombrar_archivo:(src, dst)` | Renombra un archivo. |
| `tamano_archivo:(var, ruta)` | Tamaño en bytes. |
| `crear_carpeta:(ruta)` | Crea una carpeta (recursivo). |
| `eliminar_carpeta:(ruta)` | ⚠️ Borra la carpeta y todo su contenido. |
| `leer_lineas:(var, ruta)` | Lee el archivo como lista de líneas. |
| `escribir_lineas:(ruta, lista)` | Escribe una lista como líneas. |
| `agregar_archivo:(ruta, texto)` | Añade texto al final del archivo. |
| `listar_extension:(var, dir, ".txt")` | Filtra archivos por extensión. |
| `ruta_absoluta:(var, ruta)` | Convierte a ruta absoluta. |
| `ruta_unir:(var, a, b)` | Une dos rutas. |
| `nombre_archivo:(var, ruta)` | Extrae el nombre del archivo. |
| `carpeta_padre:(var, ruta)` | Extrae la carpeta contenedora. |
| `extension_archivo:(var, ruta)` | Extrae la extensión (".txt"). |

###  JSON

| Comando | Descripción |
|---------|-------------|
| `json_dumps:(var, obj)` | Serializa un objeto → texto JSON. |
| `json_loads:(var, "texto")` | Parsea texto JSON → objeto. |
| `json_guardar:(ruta, obj)` | Guarda un objeto como JSON en archivo. |
| `json_cargar:(var, ruta)` | Carga un JSON desde archivo. |
| `json_valido:(var, "texto")` | `true` si el texto es JSON válido. |
| `json_obtener:(var, json, "a.b.c")` | Extrae un valor por ruta con puntos. |

###  Hash y codificación

| Comando | Descripción |
|---------|-------------|
| `hash_md5:(var, "texto")` | Hash MD5. |
| `hash_sha1:(var, "texto")` | Hash SHA-1. |
| `hash_sha256:(var, "texto")` | Hash SHA-256. |
| `base64_cod:(var, "texto")` | Codifica en Base64. |
| `base64_dec:(var, "base64")` | Decodifica desde Base64. |
| `uuid:(var)` | Genera un UUID v4. |

###  Expresiones regulares

| Comando | Descripción |
|---------|-------------|
| `regex_buscar:(var, "txt", "patrón")` | Todas las coincidencias → lista. |
| `regex_reemplazar:(var, "patrón", "nuevo", "txt")` | Reemplaza todas las coincidencias. |
| `regex_match:(var, "patrón", "txt")` | `true` si el patrón coincide. |
| `regex_split:(var, "patrón", "txt")` | Divide el texto con un patrón. |
| `regex_grupos:(var, "patrón", "txt")` | Grupos capturados del primer match. |
| `regex_escapar:(var, "texto")` | Escapa caracteres especiales de regex. |

###  CSV

| Comando | Descripción |
|---------|-------------|
| `csv_parsear:(var, "a,b\nc,d")` | Convierte texto CSV en matriz. |
| `csv_generar:(var, matriz)` | Convierte matriz en texto CSV. |

###  Red (limitado en HTML)

| Comando | Descripción |
|---------|-------------|
| `http_get:(var, "url")` | GET HTTP → cuerpo como texto. |
| `http_post:(var, "url", data)` | POST HTTP. |
| `http_put:(var, "url", data)` | PUT HTTP. |
| `http_delete:(var, "url")` | DELETE HTTP. |
| `url_codificar:(var, "texto")` | Codifica texto para URL. |
| `url_decodificar:(var, "urlenc")` | Decodifica texto urlencoded. |
| `resolver_dns:(var, "dominio")` | Resuelve un dominio → IP. |

> ⚠️ En la versión HTML están limitados por CORS.

###  Logging

| Comando | Descripción |
|---------|-------------|
| `log_info:("mensaje")` | Log informativo (ℹ️). |
| `log_warn:("mensaje")` | Log de advertencia (⚠️). |
| `log_error:("mensaje")` | Log de error (❌). |
| `logro:("nombre")` | Registra un logro desbloqueado (🏆). |

###  Módulos

| Comando | Descripción |
|---------|-------------|
| `importar:("ruta.ez")` | Importa las funciones y variables de otro archivo `.ez`. |

---

###  Equivalencias entre idiomas

Todos los comandos funcionan en los 3 idiomas. Ejemplos frecuentes:

| Español | English | Português |
|---------|---------|-----------|
| `mostrar` | `show` | `exibir` |
| `var` | `let` | `var` |
| `si` | `if` | `se` |
| `sino` | `else` | `senao` |
| `mientras` | `while` | `enquanto` |
| `bucle` | `loop` | `loop` |
| `funcion` | `function` | `funcao` |
| `retornar` | `return` | `retornar` |
| `clase` | `class` | `classe` |
| `nuevo` | `new` | `novo` |
| `llamar` | `call` | `chamar` |
| `sumar` | `add` | `somar` |
| `restar` | `subtract` | `subtrair` |
| `multiplicar` | `multiply` | `multiplicar` |
| `dividir` | `divide` | `dividir` |
| `boton` | `button` | `botao` |
| `color` | `color` | `cor` |
| `linea` | `line` | `linha` |
| `rectangulo` | `rectangle` | `retangulo` |
| `circulo` | `circle` | `circulo` |
| `idioma` | `language` | `idioma` |
| `modo_grafico` | `video_mode` | `modo_grafico` |
| `paleta` | `palette` | `paleta` |

>  **Consejo:** puedes mezclar idiomas en el mismo archivo si cambias el idioma activo en el menú. Los comandos en español **siempre** están disponibles como forma canónica.
