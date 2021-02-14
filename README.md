# Settings.json

Configuração de ambiente no VS code, para desenvolvimento FrontEnd e BackEnd.

- Plugins VS Code
- Docker
- Alias

# Settings.json - WSL2 integrado com Linux

## Passoa a passo para instação e configuração para o ambiente

>[ Documentação oficial WSL 2 ]
https://docs.microsoft.com/pt-br/wind...​

>[ Requisistos ]
- Atualização do Windows 10 2004 (atualização de 05/2020)
- Build: 19041.208

>[ Passo-a-passo ]
1 - Ativar o WSL
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
Obs.: Reiniciar o computador

2 - Atualizar para o WSL2
2.1 - Habilitar a plataforma da máquina virtual
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
Obs.: Reiniciar o computador

2.2 - Baixar o atualizador do kernel e realizar a instalação
Link1: https://docs.microsoft.com/pt-br/wind...​
Link2 (alternativo): https://wslstorestorage.blob.core.win...​
Obs.: Reiniciar o computador

3 - Definir o WSL2 como padrão
wsl --set-default-version 2

4 - Instalar uma distribuição Linux e realizar as configurações iniciais.
Obs.: Reiniciar o computador

5 - Alguns comandos:
- Executar e acesar o WSL2: wsl
- Exibir as distros instaladas e qual versão do wsl cada uma está utilizando: wsl -l -v
- Definir uma distro instalada para usar WSL2: wsl --set-version (distro) 2
- Exibir os comandos e menu de ajuda do WSL: wsl help
>Obs.: executar os comandos no PowerShell como administrador.
