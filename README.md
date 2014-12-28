rfc-facil
=========

Libreria para calcular el Registro Federal de Contribuyentes en México (RFC) en Java.

Uso
---
Calcular el rfc de una persona física es muy sencillo:
```java
// Josue Zarzosa de la Torre nacido el 5 de Agosto de 1987
Rfc rfc = new Rfc.Builder()
            .name("Josué")
            .firstLastName("Zarzosa")
            .secondLastName("de la Torre")
            .birthday(5, 8, 1987)
            .build();

// puedes usar el rfc completo
System.out.println(rfc.toString());

// o partes de el mismo
System.out.println(rfc.homoclave);
```
License
-------

    Copyright 2014 Josué Zarzosa

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.