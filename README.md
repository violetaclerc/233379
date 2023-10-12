# 233379

Preferiría usar AddSingleton sobre AddScoped y AddTransient cuando quiero 
una única instancia compartida en toda mi aplicación. Esto mejora la 
eficiencia al reutilizar la misma instancia en lugar de crear nuevas cada 
vez. Además, es útil para objetos de configuración que no cambian y para 
compartir un estado global de manera segura. Aunque hay que tener cuidado 
para evitar problemas de concurrencia, AddSingleton ofrece simplicidad y 
rendimiento en esos casos específicos.

Estos servicios son creados la primera vez que son pedidos o por el 
desarrollador, cuando se provee una instancia de la implementación 
directamente en el contenedor). Esto quiere decir que todas las requests 
utilizan la misma instancia. Por eso preferi usar AddSingleton sobre los 
otros dos
