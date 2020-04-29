# 01 - GUI

Esta é uma parte bem pessoal para cada usuário então vou deixar aqui três sugestões de interfaces gráficas.

## XFCE4

Antes de instalarmos a interface, vamos instalar o display manager sddm (pode ser substituido por outro display manager, como o gdm)

```console
# pacman -S sddm
```

Agora vamos habilitar o display manager para quando reiniciarmos o sistema ele ja estar funcionando.

```console
# systemctl enable sddm
```

Pronto, agora podemos instalar a interface do xfce4

```console
# pacman -S xfce4 xfce4-goodies xfce4-terminal
```

## KDE Plasma

O KDE Plasma utiliza o display manager sddm, que também pode ser substituido por outro.

```console
# pacman -S sddm
# systemctl enable sddm
```

Pronto, com o sddm instalado e habilitado, podemos instalar o KDE.

```console
# pacman -S plasma konsole dolphin
```

## Gnome

O Gnome utiliza o gdm como display manager.

```console
# pacman -S gdm
# systemctl enable gdm
```

Pronto, com o gdm instalado e habilitado, podemos instalar o Gnome.

```console
# pacman -S gnome gnome-terminal nautilus gnome-tweaks gnome-control-center adwaita-icon-theme
```

Agora que você já escolheu sua interface gráfica e instalou, basta pressionar `CTRL + D` para desmontar a partição, reiniciar a máquina, remover a mídia de instalação e pronto, você acabou de instalar o ArchLinux. Espero que tenham gostado do passo a passo !
