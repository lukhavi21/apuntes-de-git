###git log
Muestra el historial de commits

`git log --oneline`
Muestra el historial en una sola linea

`git log --graph`
Muestra el historial graficamente 

`git log --oneline --graph`
Muestra el historial de commits en una linea graficamente.(Interesante)

`git log --pretty=format:"%h - %an, %ar : %s"`

Muestra el historial con el formato que indicamos.

###Limitar la salida del historial 
`git log -n`: cambiamos  la n porq cualquier numero entero, por ejemplo: `git log -3` nos mostrara los 3 commits mas recientes.

`git log --after="2019-07-05 00:00:00"` : Muestra los commits despues de la fecha especificada.

`git log --before="2019-07-05 00:00:00"`: Muestra los commits antes de la fecha especificada. 

Las banderas del comando `git log` se pueden  usar juntas segun nos convenga, por ejemplo:
`git log --after="2019-07-04 17:00:00" --before="2019-07-04 19:00:00"` 
