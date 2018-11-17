### git log
Muestra todo el historial de commits del proyecto.

`git log --oneline` Muestra los commits en una lista.

`git log --graph` Muestra los commits más graficamente incluyendo las ramas.

`git log --oneline --graph` combinación para mostrar los commits como una lista incluyendo las ramas.

`git log --pretty=format:"%h - %an, %ar : %s"` Muestra el historial con el formato que indicamos.

`git log --decorate --oneline --graph --all`
Este comando nos muestra el historial en una sola linea por commit,nos muestra en donde estamos parados HEAD, mustra graficamente las lineas de seguimiento de las ramas, y muestra todos los commit.
