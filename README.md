# acortes — tema para Oh My Posh

Tema minimalista de dos líneas.

```
~/Projects/mi-repo on  main ↑1 +2 ~3 ?1 ≡1              5:01:27 PM
➜
```

**Línea 1, izquierda**
- Path completo; `~` para home.
- Rama de git: verde si está limpia, amarilla si tiene cambios.
- Indicadores (solo cuando aplican):
  - `↑n` / `↓n`: commits ahead/behind del remoto
  - `+n` (verde): archivos staged
  - `~n` (rojo): cambios sin stage
  - `?n` (gris): archivos untracked
  - `≡n` (magenta): stashes guardados

**Línea 1, derecha**: hora en formato de 12 horas.

**Línea 2**: `➜`, verde; rojo si el último comando falló.

Usa nombres de color ANSI, así que respeta la paleta de tu terminal. Requiere una [Nerd Font](https://www.nerdfonts.com/) para el ícono de la rama.

## Instalación

```bash
git clone https://github.com/acortes-r/oh-my-posh-theme.git ~/Projects/oh-my-posh-theme
```

En `~/.zshrc`:

```bash
eval "$(oh-my-posh init zsh --config ~/Projects/oh-my-posh-theme/acortes.omp.json)"
```

O sin clonar:

```bash
eval "$(oh-my-posh init zsh --config https://raw.githubusercontent.com/acortes-r/oh-my-posh-theme/main/acortes.omp.json)"
```
