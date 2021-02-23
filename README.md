# Documentación

## Contenido
-	Shader creado en Unity usando HLSL
-	Un modelo 3D donde aplicar el shader
-	Shader basado en Lambert
-	Contiene Mapa de normales, color y textura
-	Un color principal (Albedo) que da color a toda la iluminación
-	Control desde el material la intensidad del mapa de normal
-	Cuenta con un efecto Phong, Wrap, Banded y Rim

## Desarrollo
1.	Se crea un proyecto nuevo en Unity
2.	Se crea un nuevo shader en Unlit con un modelo de luz Lambert
3.	Se descarga un modelo 3D, en mi caso proveniente de Unity Assets Store: Space Robot Kyle | 3D Robots | Unity Asset Store
4.	Se aplican los colores y texturas al shader con _Albedo y _MainTex
5.	Se añade la normal para aplicar la textura y el strenght para que juntos puedan brindarnos un efecto más realista
6.	Aplicamos el efecto Wrap para tener un control sobre las sombras y la luz
7.	Aplicamos el efecto Phong para así dar el efecto del reflejo de la luz 
8.	En este ultimo colocamos el Specular Color para el color de la luz, el Specular Power para la intensidad, el SpecularGloss para las dimensiones del brillo y el GlossSteps para agrandar los pasos requeridos para el efecto
9.	Añadimos el efecto Rim, el cual funcionará como un reflejo de luz ubicado en las orillas 
10.	Creamos un Ramp Texture, el cual nos indica qué color se toma dependiendo de la luz y así producir un efecto de caída de color para los sombreados
11.	Aplicamos el efecto Banded, para esto necesitamos los Steps de tipo rango y así producir un efecto muy estilizado de sombreado con distintas tonalidades para darle un efecto mucho más realista al modelo.
