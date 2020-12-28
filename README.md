# AndroidTrivia - starter code
============================

Starter code for Android Kotlin Fundamentals codelab 3.1: Create and add a
fragment.

## Modificaciones
-----------------

En este punto, la app se encuentra funcional. En el próximo commit estaré agregando los desafíos de la unidad. 

## Desafío Realizado
---

Agregué dos botones, uno de **Rules** y otro de **About** en la vista **fragment_title**, los cuales me llevan a las vistas correspondientes.
En las vistas **fragment_about** y **fragment_rules agregué un botón a cada una que nos lleva a la vista **fragment_game** para iniciar el jugar.
Así mismo, se configuró para que cuando se esté en el juego y se oprima la flecha de retroceso nos lleve directamente de la vista del juego a la vista **fragment_title**

## Preguntas plateadas en el codelab con sus respuestas
---

1. ¿Cómo permite que su proyecto utilice componentes de navegación?
    R/ Se agregan las dependencias para navigation-fragment-ktx y navigation-ui-ktx en el archivo build.gradle (module).

2. ¿Dónde están definidas las posibles rutas a través de su aplicación?
    R/ En un archivo (a menudo llamado `navigation.xml`)en la carpeta de `res>navegación`.

3. ¿Cuáles de las siguientes afirmaciones sobre el NavHostFragment es verdadera?
    R/ Agrega el NavHostFragment al diseño principal agregando un `<fragment>` cuyo nombre es `androidx.navigation.fragment.NavHostFragment`.

4. ¿Dónde se configura el ID de un fragmento que se utilizará en la navegación?
    R/ En el archivo de navegación del proyecto, ya sea estableciendo el atributo `ID` en el gráfico de navegación o en el archivo XML de navegación en la carpeta de `res>navegación`  .

5. La aplicación Noticias tiene una `NewsFragment` que muestra un botón `Mostrar titulares`. El objetivo es que cuando el usuario haga clic en este botón, la aplicación navegue al archivo `HeadlinesFragment`.
    ¿Qué más debe hacer para que cuando el usuario toque el botón `Mostrar titulares` , la aplicación navegue al `HeadlinesFragment`?
    R/ En el `onclickListener` para la llamada del botón `muestre títulos` en el `navigate()` controlador de navegación, pasando por la acción que conecta el `NewsFragment` al `HeadlinesFragment`.





Introduction
------------

The AndroidTrivia app asks the user trivia questions about Android development.
It makes use of the navigation component within Jetpack to move the user between
screens. Each screen is implemented as a fragment.

The app navigates using buttons, the app bar, and a navigation drawer. Because
students haven't yet learned about saving data or the Android lifecycle, the app
tries to eliminate bugs caused by configuration changes.

Prerequisites
-------------

You need to know:
- The fundamentals of Kotlin.
- How to create basic Android apps in Kotlin.
- How to open, build, and run apps with Android Studio.
- How to work with layouts.

Getting started
---------------

1. Download and run the app.

License
-------

Copyright 2019 Google, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.