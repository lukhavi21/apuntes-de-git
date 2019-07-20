# git tag
Lista las etiquetas existentes.

## git tag nombre_etiqueta
Lista las etiquetas en orden alfabetico.

## git tag -a nombre_etiqueta -m "Mensaje de la etiqueta"

Etiqueta anotada.
Se guardan en la base de datos de Git como objetos enteros. Tienen un checksum; contienen el nombre del etiquetador, correo electronico y fecha; y tienen un mensaje asociado.

``` 
git tag -l "v1.*"
```
Lista las etiquetas que coincidan con el patron especificado.