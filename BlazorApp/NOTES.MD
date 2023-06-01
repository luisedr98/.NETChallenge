# Notas de aplicaciones con blazor

En Blazor, puede agregar archivos de C# directamente al proyecto de aplicación, como en otros proyectos de .NET. Normalmente esta técnica se denomina código subyacente y usa archivos de código independientes para almacenar la lógica de la aplicación.

Para agregar código a un archivo Razor, se usan directivas.

## Directivas de código

Las directivas de código deberían resultar familiares a los desarrolladores que han usado Razor en MVC o en páginas.

Puede usar `@()` para agregar una instrucción de C# alineada con el código HTML. Si necesita más código, use la directiva `@code` para agregar varias instrucciones entre llaves.

También puede agregar una sección`@functions` a la plantilla para los métodos y las propiedades. Se agregan a la parte superior de la clase generada, donde el documento puede hacerles referencia.

La directiva `@Page` es un marcado especial que identifica un componente como una página. Puede usar esta directiva para especificar una ruta. La ruta se asigna a una ruta de atributo que el motor de Blazor reconoce para registrar la página y acceder a ella.

Puede usar el marcado `@bind` para enlazar una variable de C# a un objeto HTML. Defina la variable de C# por nombre como una cadena en el código HTML.
