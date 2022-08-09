# BasicProject
Como esto es lo primero que hago de haskell vamos a organizar algunas de las cosas.

+ Paso 0 - Instalar haskell y stack
+ Paso 1 - Instalar VSCodium (ya veremos si nos pasamos a nvim o emacs)
+ Paso 2 - Instalar las extensiones:
   + Haskell
   + Haskell GHCi Debug Adapter Phoityne (necesita que luego instalemos stack dsfdsafdsa)
   + Haskell Syntax Highlight
   + Haskell-linter

## Crea un proyecto con stack

`stack new --resolver=lts-18.28 BasicProject`

El resolver se saca de [stackage](https://www.stackage.org/) en función del GHCI que has instalado y del soporte que da la extensión de "haskell". Asegurate
de que coges un lts que corresponda a un GHCI con soporte completo.

En este momento el GHC más moderno que tiene soporte completo es 8.10.7 --> vamos a [stackage](https://www.stackage.org/) y vemos que le corresponde el lts 18.28

De ahí sale el número

## Ve a src/Lib.hs

Una vez que el proyecto está creado vas en VSCodium a src/Libs.hs y se pone a bajar todas las cosas que necesita... paciencia

### Carga Libs.hs

`stack ghci src/Lib.hs`

Esto nos permite ejecutar "someFunc" **pero** si cambiamos algo hay que 

+ GUARDAR el archivo
+ `:re` en ghci

Para salir usamos `:q`