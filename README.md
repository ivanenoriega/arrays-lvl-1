# arrays-lvl-1

Ejercicios basicos sobre arrays.

## 1) Identificar el mes

1. Crear un array con los meses del año ej: `["enero", "febrero"...]`
2. Crea una funcion llamada `identificarMes` que reciba como parametro un numero, correspondiente a un mes. Si el mes existe disparar un `alert()` con el mensaje `El mes ingresado es: \$mes_del_año.`. si no existe, devolvemos otro `alert()` que nos diga `El mes ingresado no es correcto.`.

### Pruebas:

1. identificarMes(1) `>>>` El mes ingresado es: Enero.
2. identificarMes(6) `>>>` El mes ingresado es: Junio.
3. identificarMes(0) `>>>` El mes ingresado no es correcto.
4. identificarMes('uno') `>>>` alert: El mes ingresado no es correcto.

## 2) Detecar array

1. Crear una funcion llamada `esArray` que reciba un parametro y detecte si el parametro es o no un `array`. Si es un array debera retornar _(return)_ el valor `true`, si no lo es `false`. Tip: Existen muchas formas de hacer esta validacion, las mas comunes son `Array.isArray()` y `toString.call()`. Has pruebas con ambas para ver que devuelven.

### Pruebas:

1. esArray([]) `>>>` true
2. esArray([1, 2, 3]) `>>>` true
3. esArray(["2", [2]]) `>>>` true
4. esArray("dos") `>>>` false
5. esArray(10) `>>>` false
6. esArray(null) `>>>` false

## 3) Primer elemento

1. Crear una funcion llamada `primerElemento` que reciba un parametro y si ese parametro es un array devuelva el primer elemento del mismo. Utilizar la funcion `esArray` para validar que es un array, si lo es devolver el primer elemento (indice 0) del mismo, si no lo es, devolver `false`.

### Pruebas:

1. primerElemento([10, 2, 4]) `>>>` 10
2. primerElemento([[ ], 2, 3]) `>>>` []
3. primerElemento([[2, 3, 4], 2, 3]) `>>>` [2, 3, 4]
4. primerElemento("test") `>>>` false

## 4) Elemento n

1. Crear una funcion llamada `elementoN` que reciba dos parametros, el primer parametro es un array y el segundo un numero. La funcion debe devolver el elemento del array (primer parametro) en base al numero (segundo parametro). Crear validaciones para verificar que el primer parametro sea un array y el segundo un numero, en caso de que alguna de estas validaciones se verdadera devolver `false`.

### Pruebas:

1. elementoN([1, 2, 3, 4], 1) `>>>` 2
2. elementoN(["uno", "dos", "tres"], 2) `>>>` tres
3. elementoN([[1, 2, 3], 5, 6], 0) `>>>` [1, 2, 3]
4. elementoN("array", "numero") `>>>` false
5. elementoN([], "numero") `>>>` false
6. elementoN("array", 4) `>>>` false
