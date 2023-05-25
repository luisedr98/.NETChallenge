# Contoso Pizza Api

# Compilación y ejecución de la API web terminada

1. Ejecute el siguiente comando para compilar e iniciar la API web: `dotnet run`
2. Ejecutar en el terminal el comando `httprepl https://localhost:{PORT}` donde {PORT} es el puerto en el que se ejecuta la api
3. Ejecutar el comando `connect https://localhost:{PORT}`
4. Ir al punto de conección de la api mediante el comando `cd Pizza` y ver las acciones de la api con el comando `ls`

La lista de acciones de la api se muestran de la siguiente manera:

<code>
<pre>https://localhost:{PORT}/Pizza> ls
. [GET|POST]
.. []
{id} [GET|PUT|DELETE]</pre>
</code>

## Realizar acciones mediante httprel

5. Realice una solicitud POST para agregar una nueva pizza en HttpRepl usando el comando siguiente:

<code><pre>post -c "{"name":"Hawaii", "isGlutenFree":false}"</pre></code>

6. Actualice la nueva pizza Hawaii a una Hawaiian con una solicitud PUT con el siguiente comando:

<code><pre>put 3 -c "{"id": 3, "name":"Hawaiian", "isGlutenFree":false}"</pre></code>

7. Para comprobar que la pizza se ha actualizado, vuelva a ejecutar la acción GET con el siguiente comando `get 3`

8. Puede eliminar la pizza recién creada con la acción DELETE si ejecuta el siguiente comando: `delete 3`

9. Para comprobar que la pizza se ha quitado, vuelva a ejecutar la acción GET con el siguiente comando: `get`
