3. Agrega el repositorio original como remoto “upstream”:

```bash
git remote add upstream https://github.com/original-autor/repositorio-original.git
```

Puedes confirmar que quedó bien con:

```bash
git remote -v
```

4. Haz tus modificaciones personalizadas (íconos, textos, etc.)

Haz commit de los cambios normalmente.

5. Para actualizar desde el original (upstream) en el futuro:

```bash
git fetch upstream
git merge upstream/main
```

O si usas rebase para mantener un historial más limpio:

```bash
git fetch upstream
git rebase upstream/main
```

(Asegúrate de cambiar main si la rama principal tiene otro nombre como master o dev.)

6. Soluciona conflictos si hay

Git te dirá si hay conflictos entre tus cambios y las actualizaciones del upstream. Puedes resolverlos manualmente y luego hacer commit.

7. Sube los cambios a tu fork en GitHub:

```bash
git push origin main
```

8. Redespliega tu app en tu servidor

Usa el código actualizado desde tu repositorio.