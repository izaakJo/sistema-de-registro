<h1> sistema de registro</h1>
- estado de proyecto; en construccion.

para ejecutar el sistema, debes poner
```npm install react```
Imagina que estás trabajando en un proyecto que ya está configurado en un repositorio de origen, y deseas colaborar con este proyecto. Con git clone, es posible crear una copia de desarrollo en un repositorio local, y todos los cambios que realices van a ser gestionados a partir de este repositorio. El comando git clone es usado para seleccionar un repositorio existente y crear un clon o una copia de él en un repositorio local.

El comando git clone crea una copia de un repositorio git existente, y este repositorio puede ser local o remoto. Además, esta copia es un repositorio git completo, con tu propio historial, gestionamiento de tus propios archivos y es un ambiente aislado como un todo del repositorio original.

Por comodidad, la clonación crea una conexión remota que apunta al repositorio original. Y es esta conexión la que facilita mucho la interacción con el repositorio central. Puedes consultar un ejemplo demostrando el git clone aquí.

Con el git clone también puedes clonar el repositorio para una carpeta específica:
```git clone <repositorio> <mi-proyecto-clone>```
El repositorio localizado en repositorio es clonado para una carpeta llamada:
```mi-proyecto-clone```
También puedes configurar el git clone y clonar el repositorio desde una branch específica, diferente a la original, de esta manera:
```git clone -branch new_feature <repositorio>```

<h1>Para saber más: Git Log</h1>

Si deseas verificar el historial de cambios, los mensajes de commit, el nombre de la persona autora del commit y otras informaciones sobre el proyecto, hay un comando de git que te puede ayudar. Este comando es git log.
Como ya sabemos, los commits poseen hashs que los identifican de una manera única, es decir, no existen dos commits con el mismo hash. Con git log podemos ver el hash y muchas otras informaciones del commit.
Podemos visualizar todos los commits, uno en cada línea con el comando:
```git log –oneline```
Si, en lugar de menos informaciones, queremos ver más, como las alteraciones del commit, podemos usar:
```git log -p```
También podemos buscar las informaciones de la persona autora del commit con el comando:
```git log --author="user_name"```
Y buscar informaciones por fecha:
```git log --since=1.month.ago --until=1.day.ago```
En el comando anterior, estamos buscando las informaciones del commit desde hace un mes hasta hace un día.
Tu también puedes formatear la visualización de las informaciones del commit con el comando:
```git log --pretty="format:%h %s"```
