# Investigaciones

En el siguiente archivo se iran anexando los elementos del cual debemos saber los significados. 

1. PARADIGMA NO RELACIONAL: No se implementan los mecanismos de consistencia como en las bases de datos relacionales, donde la confirmación de un cambio implica una comunicación de los mismos a todos los nodos que se relacionen. Esta flexibilidad hace que la consistencia se dé, eventualmente, cuando no se hayan modificado los datos durante un periodo de tiempo. Generalmente se distribuyen los datos mediante mecanismos de tablas de hash distribuida (DHT). Tiene tolerancia a fallos y redundancia. 

2. CRUD DE MONGO: En mongo, una base de datos sigue siendo una base de datos las TABLAS de convierten en COLECCIONES, las COLUMNAS son RECORDS y no hay columnas.  
    * Aquí no se crean bases de datos, se usan, entonces para crear una base de datos se hace lo siguiente:
        - use nombredelabasededatos
        - use animals;
    
    * Para agregar infrormación a la base de datos:
        - db.collection.save()
        - Ejemplo: > db.animals.save({'animal':'cat', 'name':'fluffy', 'type':'long-haired', 'owner':'Anna'});

    * Para checar informacion, parecido a un SELECT en SQL:
        - db.collection.find();
        - EJEMPLO > db.animals.find();
{ "_id" : ObjectId("4ebb8fd68f7aaffc5d287383"), "animal" : "cat", "name" : "fluffy", "type" : "long-haired", "owner" : "Anna" }
        - O bien, podemos poner un "WHERE": > db.animals.find({'animal':'cat'});
        

3. NoSQL:  Los datos almacenados no requieren estructuras fijas como tablas, normalmente no soportan operaciones JOIN, ni garantizan completamente ACID (atomicidad, consistencia, aislamiento y durabilidad), y habitualmente escalan bien horizontalmente. 
Por lo general, los investigadores académicos se refieren a este tipo de bases de datos como almacenamiento estructurado, término que abarca también las bases de datos relacionales clásicas. A menudo, las bases de datos NoSQL se clasifican según su forma de almacenar los datos, y comprenden categorías como clave-valor, las implementaciones de BigTable, bases de datos documentales, y Bases de datos orientadas a grafos.

4. SCAFFOLD:


5. PROXY PASS: gestionan el salto y la vuelta del servidor de front-end al de back-end.

       






