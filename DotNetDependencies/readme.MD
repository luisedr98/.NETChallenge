# Instalación de dependencias en .NET

## Gestión de dependencias

Comandos para la gestión de dependencias en .NET

- Para agregar dependencias y actualizar
  `dotnet add package <paquete>`
- Para conocer el listado de dependecias disponibles en el proyecto
  `dotnet list package <paquete>`
- Para la eliminación de dependencias
  `dotnet remove package <paquete>`
- Para conocer las dependecias obseletas y conocer las nuevas versiones
  `dotnet list package --outdated`

## Gestión de dependencias por versiones

1. lastest `dotnet add package <paquete>`
2. versión específica `dotnet add package <paquete> --version <version>
3. preliminar `dotnet add package --prerelease`

## Docuementación de MS

[[Creación de un proyecto de .NET y trabajo con dependencias]][1]
[1]: https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/?WT.mc_id=cloudskillschallenge_150AAE80-E46B-4A07-894A-5247FCDFCBAD "Creación de un proyecto de .NET y trabajo con dependencias"
