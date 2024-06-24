# jslib
**ES** | [PT](README.md) | [EN](README-en.md) 

Métodos de la clase JSLib disponibles para uso en los scripts del programa Holyrics.

Es posible utilizar la variable ```jslib``` o la variable ```h``` para acceder a los métodos disponibles.

Por ejemplo:

```
jslib.log('exemplo');
h.log('exemplo');
```
---

- [Métodos](#métodos)
  - [log](#logobj)
  - [log](#logkey--null-obj-args--null)
  - [log.enable](#logenablekey)
  - [log.enableAll](#logenableall)
  - [log.isEnabled](#logisenabledkey)
  - [log.setShowLogKey](#logsetshowlogkeyvalue)
  - [log.isShowLogKey](#logisshowlogkey)
  - [sleep](#sleeptime)
  - [base64Encode](#base64encodebytes)
  - [base64Decode](#base64decodestr)
  - [base64DecodeAsString](#base64decodeasstringstr-charset--utf8)
  - [hash](#hashhashname-data)
  - [hashBytes](#hashbyteshashname-data)
  - [checksum](#checksumchecksumname-data)
  - [md5](#md5value)
  - [md5Str](#md5strvalue)
  - [sha256](#sha256value)
  - [sha256Str](#sha256strvalue)
  - [sha512](#sha512value)
  - [sha512Str](#sha512strvalue)
  - [getClipboard](#getclipboard)
  - [normalize](#normalizestr)
  - [store](#storekey-value)
  - [restore](#restorekey)
  - [setGlobal](#setglobalkey-value-ttl--0)
  - [getGlobal](#getglobalkey-default--null)
  - [setGlobalNext](#setglobalnextkey-values-ttl--0)
  - [getGlobalAndSet](#getglobalandsetkey-default--null-newvalue)
  - [getGlobalAndSetNext](#getglobalandsetnextkey-values)
  - [setGlobalNextAndGet](#setglobalnextandgetkey-values)
  - [random](#randommin-max-keysaferepeat--null)
  - [random](#randomx-y-z)
  - [startTimer](#starttimerkey--default)
  - [getTimer](#gettimerkey--default)
  - [getTimerMillis](#gettimermilliskey)
  - [getTimerSeconds](#gettimersecondskey)
  - [startCountdown](#startcountdownkey--default-seconds)
  - [getCountdown](#getcountdownkey--default)
  - [getCountdownMillis](#getcountdownmilliskey)
  - [getCountdownSeconds](#getcountdownsecondskey)
  - [getPlaylistInfo](#getplaylistinfo)
  - [getPlayer](#getplayer)
  - [scriptAction](#scriptaction)

---

Continúo traduciendo el resto del documento para ofrecerte la traducción completa.

Aquí está la traducción completa del documento:

---

# jslib
**PT** | [EN](README-en.md)

Métodos de la clase JSLib disponibles para uso en los scripts del programa Holyrics.

Es posible utilizar la variable ```jslib``` o la variable ```h``` para acceder a los métodos disponibles.

Por ejemplo:

```
jslib.log('ejemplo');
h.log('ejemplo');
```
---

- [Métodos](#métodos)
  - [log](#logobj)
  - [log](#logkey--null-obj-args--null)
  - [log.enable](#logenablekey)
  - [log.enableAll](#logenableall)
  - [log.isEnabled](#logisenabledkey)
  - [log.setShowLogKey](#logsetshowlogkeyvalue)
  - [log.isShowLogKey](#logisshowlogkey)
  - [sleep](#sleeptime)
  - [base64Encode](#base64encodebytes)
  - [base64Decode](#base64decodestr)
  - [base64DecodeAsString](#base64decodeasstringstr-charset--utf8)
  - [hash](#hashhashname-data)
  - [hashBytes](#hashbyteshashname-data)
  - [checksum](#checksumchecksumname-data)
  - [md5](#md5value)
  - [md5Str](#md5strvalue)
  - [sha256](#sha256value)
  - [sha256Str](#sha256strvalue)
  - [sha512](#sha512value)
  - [sha512Str](#sha512strvalue)
  - [getClipboard](#getclipboard)
  - [normalize](#normalizestr)
  - [store](#storekey-value)
  - [restore](#restorekey)
  - [setGlobal](#setglobalkey-value-ttl--0)
  - [getGlobal](#getglobalkey-default--null)
  - [setGlobalNext](#setglobalnextkey-values-ttl--0)
  - [getGlobalAndSet](#getglobalandsetkey-default--null-newvalue)
  - [getGlobalAndSetNext](#getglobalandsetnextkey-values)
  - [setGlobalNextAndGet](#setglobalnextandgetkey-values)
  - [random](#randommin-max-keysaferepeat--null)
  - [random](#randomx-y-z)
  - [startTimer](#starttimerkey--default)
  - [getTimer](#gettimerkey--default)
  - [getTimerMillis](#gettimermilliskey)
  - [getTimerSeconds](#gettimersecondskey)
  - [startCountdown](#startcountdownkey--default-seconds)
  - [getCountdown](#getcountdownkey--default)
  - [getCountdownMillis](#getcountdownmilliskey)
  - [getCountdownSeconds](#getcountdownsecondskey)
  - [getPlaylistInfo](#getplaylistinfo)
  - [getPlayer](#getplayer)
  - [scriptAction](#scriptaction)

---

## Métodos

### log(obj)
Registra un mensaje en la consola.

**Parámetros:**
- `obj` (_Object_): El objeto a registrar.

### log(key = null, obj, args = null)
Registra un mensaje con una clave específica en la consola.

**Parámetros:**
- `key` (_String_): La clave del mensaje.
- `obj` (_Object_): El objeto a registrar.
- `args` (_Array_): Argumentos adicionales.

### log.enable(key)
Habilita el registro de mensajes para una clave específica.

**Parámetros:**
- `key` (_String_): La clave del mensaje.

### log.enableAll()
Habilita el registro de todos los mensajes.

### log.isEnabled(key)
Verifica si el registro de mensajes está habilitado para una clave específica.

**Parámetros:**
- `key` (_String_): La clave del mensaje.

**Retorno:**
- (_Boolean_): `true` si está habilitado, `false` de lo contrario.

### log.setShowLogKey(value)
Establece si se debe mostrar la clave del mensaje en los registros.

**Parámetros:**
- `value` (_Boolean_): `true` para mostrar la clave, `false` de lo contrario.

### log.isShowLogKey()
Verifica si se está mostrando la clave del mensaje en los registros.

**Retorno:**
- (_Boolean_): `true` si se muestra, `false` de lo contrario.

### sleep(time)
Detiene la ejecución durante un tiempo específico.

**Parámetros:**
- `time` (_Number_): El tiempo en milisegundos.

### base64Encode(bytes)
Codifica un conjunto de bytes en una cadena Base64.

**Parámetros:**
- `bytes` (_Array_): Los bytes a codificar.

### base64Decode(str)
Decodifica una cadena Base64 en bytes.

**Parámetros:**
- `str` (_String_): La cadena Base64 a decodificar.

### base64DecodeAsString(str, charset = 'utf8')
Decodifica una cadena Base64 en una cadena utilizando un conjunto de caracteres específico.

**Parámetros:**
- `str` (_String_): La cadena Base64 a decodificar.
- `charset` (_String_): El conjunto de caracteres a utilizar.

### hash(hashName, data)
Genera un hash para los datos especificados utilizando el algoritmo dado.

**Parámetros:**
- `hashName` (_String_): El nombre del algoritmo de hash.
- `data` (_String_): Los datos a hashear.

### hashBytes(hashName, data)
Genera un hash en bytes para los datos especificados utilizando el algoritmo dado.

**Parámetros:**
- `hashName` (_String_): El nombre del algoritmo de hash.
- `data` (_Array_): Los datos a hashear.

### checksum(checksumName, data)
Genera un checksum para los datos especificados utilizando el algoritmo dado.

**Parámetros:**
- `checksumName` (_String_): El nombre del algoritmo de checksum.
- `data` (_String_): Los datos para el checksum.

### md5(value)
Genera un hash MD5 para el valor especificado.

**Parámetros:**
- `value` (_String_): El valor a hashear.

### md5Str(value)
Genera un hash MD5 en forma de cadena para el valor especificado.

**Parámetros:**
- `value` (_String_): El valor a hashear.

### sha256(value)
Genera un hash SHA-256 para el valor especificado.

**Parámetros:**
- `value` (_String_): El valor a hashear.

### sha256Str(value)
Genera un hash SHA-256 en forma de cadena para el valor especificado.

**Parámetros:**
- `value` (_String_): El valor a hashear.

### sha512(value)
Genera un hash SHA-512 para el valor especificado.

**Parámetros:**
- `value` (_String_): El valor a hashear.

### sha512Str(value)
Genera un hash SHA-512 en forma de cadena para el valor especificado.

**Parámetros:**
- `value` (_String_): El valor a hashear.

### getClipboard()
Obtiene el contenido actual del portapapeles.

**Retorno:**
- (_String_): El contenido del portapapeles.

### normalize(str)
Normaliza una cadena eliminando acentos y caracteres especiales.

**Parámetros:**
- `str` (_String_): La cadena a normalizar.

### store(key, value)
Almacena un valor con una clave específica.

**Parámetros:**
- `key` (_String_): La clave del valor.
- `value` (_String_): El valor a almacenar.

### restore(key)
Restaura un valor almacenado con una clave específica.

**Parámetros:**
- `key` (_String_): La clave del valor.

**Retorno:**
- (_String_): El valor almacenado.

### setGlobal(key, value, ttl = 0)
Establece un valor global con una clave específica y un tiempo de vida (TTL).

**Parámetros:**
- `key` (_String_): La clave del valor.
- `value` (_String_): El valor a establecer.
- `ttl` (_Number_): El tiempo de vida en segundos.

### getGlobal(key, default = null)
Obtiene un valor global por su clave, devolviendo un valor predeterminado si no se encuentra.

**Parámetros:**
- `key` (_String_): La clave del valor.
- `default` (_Any_): El valor predeterminado a devolver si no se encuentra.

**Retorno:**
- (_Any_): El valor global.

### setGlobalNext(key, values, ttl = 0)
Establece el siguiente valor global en una lista con una clave específica y un tiempo de vida (TTL).

**Parámetros:**
- `key` (_String_): La clave del valor.
- `values` (_Array_): Los valores a establecer.
- `ttl` (_Number_): El tiempo de vida en segundos.

### getGlobalAndSet(key, default = null, newValue)
Obtiene un valor global y establece un nuevo valor para la misma clave.

**Parámetros:**
- `key` (_String_): La clave del valor.
-

 `default` (_Any_): El valor predeterminado a devolver si no se encuentra.
- `newValue` (_Any_): El nuevo valor a establecer.

**Retorno:**
- (_Any_): El valor global anterior.

### getGlobalAndSetNext(key, values)
Obtiene un valor global y establece el siguiente valor en una lista para la misma clave.

**Parámetros:**
- `key` (_String_): La clave del valor.
- `values` (_Array_): Los valores a establecer.

**Retorno:**
- (_Any_): El valor global anterior.

### setGlobalNextAndGet(key, values)
Establece el siguiente valor global en una lista y obtiene el nuevo valor para la misma clave.

**Parámetros:**
- `key` (_String_): La clave del valor.
- `values` (_Array_): Los valores a establecer.

**Retorno:**
- (_Any_): El nuevo valor global.

### random(min, max, keySafeRepeat = null)
Genera un número aleatorio entre `min` y `max`.

**Parámetros:**
- `min` (_Number_): El valor mínimo.
- `max` (_Number_): El valor máximo.
- `keySafeRepeat` (_String_): La clave para evitar repeticiones.

**Retorno:**
- (_Number_): El número aleatorio.

### random(x, y, z)
Genera un número aleatorio entre `x`, `y` y `z`.

**Parámetros:**
- `x` (_Number_): El primer valor.
- `y` (_Number_): El segundo valor.
- `z` (_Number_): El tercer valor.

**Retorno:**
- (_Number_): El número aleatorio.

### startTimer(key = 'default')
Inicia un temporizador con una clave específica.

**Parámetros:**
- `key` (_String_): La clave del temporizador.

### getTimer(key = 'default')
Obtiene el valor del temporizador con una clave específica.

**Parámetros:**
- `key` (_String_): La clave del temporizador.

**Retorno:**
- (_Number_): El valor del temporizador en milisegundos.

### getTimerMillis(key)
Obtiene el valor del temporizador en milisegundos.

**Parámetros:**
- `key` (_String_): La clave del temporizador.

**Retorno:**
- (_Number_): El valor del temporizador en milisegundos.

### getTimerSeconds(key)
Obtiene el valor del temporizador en segundos.

**Parámetros:**
- `key` (_String_): La clave del temporizador.

**Retorno:**
- (_Number_): El valor del temporizador en segundos.

### startCountdown(key = 'default', seconds)
Inicia una cuenta regresiva con una clave específica y un tiempo en segundos.

**Parámetros:**
- `key` (_String_): La clave de la cuenta regresiva.
- `seconds` (_Number_): El tiempo en segundos.

### getCountdown(key = 'default')
Obtiene el valor de la cuenta regresiva con una clave específica.

**Parámetros:**
- `key` (_String_): La clave de la cuenta regresiva.

**Retorno:**
- (_Number_): El valor de la cuenta regresiva en milisegundos.

### getCountdownMillis(key)
Obtiene el valor de la cuenta regresiva en milisegundos.

**Parámetros:**
- `key` (_String_): La clave de la cuenta regresiva.

**Retorno:**
- (_Number_): El valor de la cuenta regresiva en milisegundos.

### getCountdownSeconds(key)
Obtiene el valor de la cuenta regresiva en segundos.

**Parámetros:**
- `key` (_String_): La clave de la cuenta regresiva.

**Retorno:**
- (_Number_): El valor de la cuenta regresiva en segundos.

### getPlaylistInfo()
Obtiene información de la lista de reproducción.

**Retorno:**
- (_Object_): La información de la lista de reproducción.

### getPlayer()
Obtiene el reproductor actual.

**Retorno:**
- (_Object_): El reproductor.

### scriptAction()
Ejecuta una acción de script.

---

## Configuración de Estilos de Texto

Para mostrar un texto con formato avanzado, inicia el texto con **<styled>**.

Etiquetas HTML disponibles:

```
<styled>
<b>negrita</b>
<i>itálica</i>
<u>subrayado</u>
<color:0000FF>color de la fuente</color>
<font:Times New Roman>nombre de la fuente</font>
<size:70>tamaño relativo de la fuente 70%</size>
```

---
