Laboratorio | Revisión del estudio de caso de aprendizaje automático
En este laboratorio, utilizará learningSet.csvel archivo que ya ha clonado en las actividades de hoy.
Instrucciones
Complete los siguientes pasos en las columnas categóricas del conjunto de datos:

Comprobar si hay valores nulos en todas las columnas

Excluya las siguientes variables consultando las definiciones. Cree una nueva lista vacía llamada drop_list. Anexaremos esta lista y luego eliminaremos todas las columnas de esta lista más adelante:

OSOURCE- No se proporcionan definiciones de símbolos, demasiadas categorías
ZIP CODE- ya estamos incluyendo el estado
Identificar columnas en las que faltan más del 85 % de valores

Eliminar esas columnas del marco de datos

Reducir la cantidad de categorías en la columna GENDER. La columna solo debe tener "M" para hombres, "F" para mujeres y "otro" para el resto.

Tenga en cuenta que hay algunos valores nulos en la columna. Primero reemplazaremos esos valores nulos con el código que se muestra a continuación:
print(categorical['GENDER'].value_counts())
categorical['GENDER'] = categorical['GENDER'].fillna('F')
