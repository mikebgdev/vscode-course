<p align="center">
  <a href="https://fernando-herrera.com/" target="blank"><img src="https://devtalles.com/images/vscode.png" width="100" alt="Nest Logo" /></a>
</p>

# Curso de VSCode
Un repositorio donde aprenderemos un par de trucos para trabajar rápidamente con Visual Studio Code.

También hay un par de extensiones bastante útiles que les recomiendo de entrada

* [Descargar VSCode - Sitio Oficial](https://code.visualstudio.com/)

## Extensiones

# Indispensables:

* [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)

* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

* [Activitus Bar](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.activitusbar)

* [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)

* [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)

* [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)


## Tema usado durante el curso

* [Aura Theme](https://marketplace.visualstudio.com/items?itemName=DaltonMenezes.aura-theme)


# Wallpapers que uso
[Wallpapers Developer](https://drive.google.com/drive/folders/1ItU8rbSGJjnh2USOBGwaCo9nYKifPJ6m?usp=sharing)

<!-- repository-quality-20261101 -->
 ## Comprobaciones y publicación

 La verificación del repositorio está en `ci/verify.sh`. Necesita las dependencias de desarrollo descritas arriba; no utiliza datos ni credenciales de producción.

 ```sh
 bash ci/verify.sh
 ```

 El workflow **Quality** comprueba secretos y después ejecuta esas comprobaciones en pushes a la rama principal y en pull requests. El escaneo usa Gitleaks 8.30.1 con descarga verificada por SHA256; examina el historial Git disponible y el directorio actual. No imprime valores de secretos. Para la revisión completa local, usar un clon con historial completo y ejecutar `bash ci/check_secrets.sh`; se puede indicar `GITLEAKS_BIN` con esa versión instalada.

 La existencia del archivo de workflow no acredita que el runner esté disponible ni que la revisión haya pasado. Antes de integrar, comprobar los resultados **Secrets** y **Verify** del mismo SHA. Este workflow no despliega servicios. Conservar el procedimiento de entrega y rollback específico del proyecto.


## Aplicación de ejemplo y ejercicios

La entrada ejecutable es `src/main.ts`, con `src/counter.ts` y los tipos de Vite. Los directorios numerados son ejercicios de edición: conservan fragmentos incompletos, repeticiones y plantillas para practicar el editor; no forman parte de la aplicación Vite. El build comprueba la aplicación, no declara compilables todos esos fragmentos. Instalación: `npm ci`; desarrollo: `npm run dev`; entrega estática: `npm run build`, en `dist/`.

El README referencia el curso de Fernando Herrera/DevTalles. Confirmar la procedencia y los permisos de los ejercicios antes de atribuirse o relicenciar ese material; la recomendación de licencia solo alcanza código propio comprobado.

<!-- license-adopted-20261101 -->
## Licencia

**MIT**, con el alcance indicado en [docs/LICENSING.md](docs/LICENSING.md). El texto completo está en [LICENSE](LICENSE). La concesión cubre las aportaciones propias; los recursos y componentes de terceros conservan sus licencias y atribuciones.
