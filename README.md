# Práctica Evaluable

mkdir practica_evaluable
cd practica_evaluable
git init
echo "Contenido del documento1" > documento1.txt
echo "Contenido del documento2" > documento2.txt
git add documento1.txt documento2.txt
git commit -m "Añadir documentos 1 y 2"
echo "Nuevas líneas en documento1" >> documento1.txt
git add documento1.txt
git commit -m "Actualizar documento1"
echo "Cambios en documento2" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2"
git reset --hard HEAD^
echo "Contenido del documento3" > documento3.txt
git add documento3.txt
git commit -m "Añadir documento3"
git revert HEAD^
git revert HEAD^
git remote add origin https://github.com/tu-usuario/practica_evaluable.git
git push -u origin main
git checkout -b mirama
echo "Contenido de rama1" > rama1.txt
echo "Contenido de rama2" > rama2.txt
git add rama1.txt rama2.txt
git commit -m "Añadir rama1.txt y rama2.txt"
git checkout master
git merge mirama
git branch -d mirama
git push origin master
git tag -a V1 -m "Versión 1"
git push origin --tags
git clone https://github.com/tu-usuario/practica_evaluable.git practica_evaluable_2
cd practica_evaluable_2
git checkout -b mirama
echo "Cambios en mirama" >> documento1.txt
git add documento1.txt
git commit -m "Actualizar documento1 en mirama"
git push -u origin mirama
git checkout master
echo "Cambios en master" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2 en master"
git push origin master
git merge mirama
git branch -d mirama
git push origin master
echo "Nuevos cambios en documento2" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2"
git checkout -b mirama
echo "Cambios en mirama en documento2" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2 en mirama"
git checkout master
git merge mirama
git checkout -b mirama
echo "Cambios en mirama en documento2" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2 en mirama"
git checkout master
echo "Cambios en master en documento2" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2 en master"
git checkout mirama
echo "Cambios en mirama en documento2" >> documento2.txt
git add documento2.txt
git commit -m "Actualizar documento2 en mirama"
git checkout master
git merge mirama
<<<<<<< HEAD
Cambios en master en documento2
=======
Cambios en mirama en documento2
>>>>>>> mirama
git add documento2.txt
git commit -m "Resolver conflicto en documento2.txt"
git merge --continue
git push origin master
echo "# Práctica Evaluable" > README.md
git add README.md
git commit -m "Añadir README.md"
git push origin master
git pull origin master
