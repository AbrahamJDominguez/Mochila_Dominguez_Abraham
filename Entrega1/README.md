mkdir peliculas
cd peliculas
mkdir infantiles accion terror comedia romanticas
touch infantiles/{intenzamente.txt,"el juego del miedo.xls","rapido y furioso.pdf","titanic.jpg"}
touch accion/{"smooth criminal.txt","diario de una pasion.js","el hexorcista.xls",cars.jpg}
touch terror/{"la dama y el bagavundo.png","yo antes de ti.xls","que paso ayer.pdf","we will rock you.js"}
touch comedia/{madagaskar.js,"orgullo y prejuicio.txt","it.xls","mision imposible.png"}
touch romantica/{pocahontas.jpg,annabelle.js,"los vengadores.js","la mascara.js"}
ls -R

/* Si, se pueden crear todas las carpetas de un solo comando
También se pueden crear todos los archivos de un solo comando */

cd ..
mkdir peliculas/romanticas/prueba
cd peliculas/romanticas
mkdir ../accion/prueba2

cd ..
mv {accion/cars.jpg,terror/"la dama y el bagavundo.png",madagaskar.js} infantiles
mv {infantiles/"rapido y furioso.pdf",comedia/"mision imposible.png","los vengadores.js"} accion
mv {infantiles/"el juego del miedo.xls",accion/"el hexorcista.xls",comedia/it.xls,romanticas/annabelle.js} terror
mv {terror/"que paso ayer.pdf","la mascara.js"} comedia
mv {infantiles/titanic.jpg,accion/"diario de una pasion.js",terror/"yo antes de ti.xls",comedia/"orgullo y prejuicio.txt"} romanticas
cd ..
mv infantiles/intenzamente.js infantiles/intensamente.js
mv infantiles/"la dama y el bagavungo.png" infantiles/"la dama y el vagabundo.png"
mv infantiles/madagaskar.js infantiles/madagascar.js
mv terror/"el exorcista.xls" terror/"el exorcista.xls"
rm peliculas/{accion/"smooth criminal.txt",terror/"we will rock you"}
touch peliculas/accion/noBorrar.js
cd peliculas
mv accion/prueba2/noBorrar.js romanticas/prueba
cd ..
touch camada5.txt
cd peliculas 
mv terror/it.xls infantiles
rm ../camada5.txt
rmdir -r romanticas
