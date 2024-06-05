# Trucos Git
## Deshacer el ultimo commit, manteniendo cambio
```bash
git reset --soft HEAD~1
```
## Modificar commit, sin crear nuevo commit usando --amend 
**--amend solo funciona en el ultimo commit siempre y cuando no se haya subido al repo**
```bash

# Añade los archivos con modificaciones
# que quieres añadir al commit anterior
git add src/archivo-con-cambios.js

# Vuelve a hacer el commit con el parámetro amend
git commit --amend -m "Mensaje del commit"
```