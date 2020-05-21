# 01 - Pacotes essenciais

Bom, agora chegamos na parte que de fato vamos instalar nosso sistema, vamos em frente.

## Mirrors

Os mirrors estão localizados em `/etc/pacman.d/mirrorlist` e são utilizados para fazermos os downloads dos pacotes no nosso sistema, então você pode querer alterar e
deixar o mirrors brasileiros com maior prioridade pois quando instalarmos nosso sistema essa lista de mirrors será copiada.

Para fazer a alteração é bem simples, vamos usar o `reflector` para isso mas antes iremos instala-lo.

```console
# pacman -Sy reflector
```

Depois de termos instalado o reflector, iremos executar o seguinte comando:

```console
# reflector --country Brazil --age 24 --sort rate --save /etc/pacman.d/mirrorlist
```
*Obs: caso queria trocar o país de onde os mirrors serão pegos basta alterar no comando* 

Esse comando irá trazer pra gente todos os mirros do Brasil pela velocidade de download e irá sobrescrever o arquivo dos mirrors.

Agora com nossos mirrors brasileiros com maior prioridade, podemos continuar com a instalação.

## Pacotes Essenciais

Chegou a hora de instalarmos de fato o conteúdo do nosso sistema, para fazermos isso nós utilizamos o comando `pacstrap`, este comando é o responsável por baixar e instalar os pacotes.

Nós vamos instalar os pacotes base, linux e linux-firmware dentro da pasta onde montamos nosso sistema.

```console
# pacstrap /mnt base linux linux-firmware
```

- O pacote _base_ contém todo o necessário para que nosso sistema funcione.
- O pacote _linux_ é o nosso kernel, então se você deseja instalar outro kernel substitua-o.
- O pacote _linux-firmware_ não contém pacotes específicos, então se deseja instalar algum firmware em especial você deverá passar juntamente a esta lista de pacote.

Esta parte costuma demorar um pouco, isso vai de acordo com a sua internet, então enquanto você espera baixar e instalar os pacotes da uma passada na [He4rt Developers](https://discord.io/He4rt) ou da uma olhada nos outros tutoriais [4noobs](https://github.com/he4rt/4noobs) temos conteúdo de qualidade para vocês e te vejo no [próximo arquivo](../4-Configuracao/1-Fstab.md) :)

---

### Referências

[Wiki - Instalação](https://wiki.archlinux.org/index.php/Installation_guide#Installation)

[Wiki - Reflector](https://wiki.archlinux.org/index.php/Reflector_(Portugu%C3%AAs))