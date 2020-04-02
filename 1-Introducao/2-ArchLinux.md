# 02 - O que é ArchLinux ?

O ArchLinux é uma distribuição GNU/Linux que utiliza a arquitetura x86_64 de uso geral desenvolvida independentemente que se empenha em fornecer as últimas versões estáveis da maioria dos softwares seguindo um modelo de lançamento contínuo (rolling-release).

## Alguns princípios

### Simplicidade

O Arch Linux define simplicidade como sem adições ou modificações desnecessárias. Ele provê softwares conforme lançado pelos desenvolvedores originais (upstream) com alterações mínimas específicas da distribuição (downstream). E as configurações destes softwares são alteraveis, como caminhos de arquivos de sistema.

### Modernidade

O Arch Linux se esforça para oferecer as versões mais recentes e estáveis de seus pacotes, assim evitando razoavelmente a quebra sistematica de pacotes. É baseeado em um sistema rolling-release, então permite uma unica instalação e upgrades contínuos. Ele também incorpora muitas das novas funcionalidades do GNU/Linux, como *systemd, LVM2, RAID, udev e initcpio (com mkinitcpio) e kernels recentes*.

### Centrado no Usuário

O Arch Linux ao contrário das outras distribuições, que geralmente tentam ser user-friendly, ele é user-centric, ou seja, ele tem a inteção de suprir as necessidades de cada usuário em vez de agradar a maior quantidade de usuários possivel.

### Versatilidade

Arch Linux é uma distribuição de propósito geral. Na instalação, nos é fornecido apenas um ambiente de linha de comando em vez de "enfiar" varios pacotes desnecessários e indesejados, assim oferecendo ao usuário a habilidade de compilar seu próprio sistema personalizado escolhendo entre os diversos pacotes de alta qualidade contidos nos repositorios 
oficiais para a arquitetura x86_64.

## Pacman

Arch funciona com o pacman, um gerenciador de pacotes leve, simples e rápido que permite atualizar todo o sistema com apenas um comando.

O pacman que é o responsavel por atualizar nosso sistema, instalar e remover pacotes com comandos simples, e ele é um gerenciador completo com todas as depencências necessarias.

Alguns comandos

Comando | Função
--- | ---
pacman -S *pacote1 pacote2 ...*| Instala os pacotes
pacman -Ss *string* | procura pacotes na base de dados, procura por nomes e descrições do pacote
pacman -Syu | atualiza todos os pacotes do sistema
pacman -R *pacote* | Remove um pacote
pacman -RS *pacote* | Remove um pacote e suas dependências que não são exigidas por outro pacote

Agora que sabemos o que é o ArchLinux podemos ir ao [próximo arquivo](../2-PreInstalacao/1-Passos.md).

---

## Referências

[Wiki - ArchLinux](https://wiki.archlinux.org/index.php/Arch_Linux)<br>
[Wiki - Pacman](https://wiki.archlinux.org/index.php/Pacman)
