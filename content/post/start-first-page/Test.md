# Mi configuración de nixos.
Esta es mi configuración de nixos, es funciona para mi caso, tiene todo lo necesario para mi escritorio, se que le falta optimizar algunas cosas, lo estare haciendo en cuanto pueda, la configuracion esta fecha con **flakes** esta dividida en distintos modulos y por programas, para que sea mas personalizable, tengo en mente pasar todo a **Miri**, pero por el momento me funciona i3, ademas que **Wayland** es relativamente joven y no tengo los conocimientos para hacer este cambio aunque ya hetenido experiencia con Wayland en otras distros, si te gusta nixos, y tengas una recommendation me puedes escribir, a mi Matrix.
#### Por que el cambio a esta Distro?
Nixos, te permite tener un sistema declarativo que se pueda replicar en cualquier maquina sin necesidad de hacer configuraciones adicionales lo cual es util para tener entornos reproducible; principalmente me gusta por las infinitas herramientas que ofrece para el desarrollo, como es los **Flakes**, la posibilidad de declarar los dotfiles en un archivos nix, personalmente me gustan los lenguajes funcionales como es nix, aun tengo que aprender muchas cosas, ya que nix tiene una curva de aprendizaje un poco empinada, pero el hecho es que es divertido lo que ofrece nix... 

## Instalación 
### Construction general 
```bash
sudo nixos-rebuild switch --flake ~/directory#user
```

### Módulos de desarrollo
Al ejecutar un modulo debemos estar en la carpeta del **Flake**
```bash
nix develop 
```