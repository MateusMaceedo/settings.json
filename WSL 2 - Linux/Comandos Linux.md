# Principais Comandos do Terminal no LINUX

## Dicas:

#### 1) Para listar todos os comandos disponiveis num terminal basta apertar TAB duas vezes, o terminal vai pergunta se você quer ver todos os comandos. Display all 3466 possibilities? (y or n)

Então basta aperta y ( yes-sim ) e todos os comandos serão listados, se apertar n ( no-não ) sera cancelado a listagem.
o numero de "possibilities" pode variar.

#### 2) Para saber mais sobre o comando basta adicionar --help na frente exemplo:

wget --help

lspci --help

obs: geralmente os helps são em ingles.

#### 3) O terminal tem sensibilidade com maiúsculas e minúsculas, tudo tem que ser digitado da maneira exata de como é escrito.

>1. ls (lista o conteúdo de um diretório)
Exemplo: $ ls


>2. ls -a (lista os diretórios, arquivos oculto e executáveis)
Exemplo: $ ls -a


>3. ls -l (Lista o conteúdo de um diretório detalhadamente)
Exemplo: $ ls -l


>4. pwd (mostra o diretório corrente)
Exemplo: $ pwd


>5. cd (muda de diretório)
Exemplo: $ cd /etc


>6. cd - (volta para o diretório anterior)
Exemplo: $ cd -


>7. cd .. (volta um diretório acima)
Exemplo: $ cd ..


>8. cd ~ (volta para seu diretório /home)
Exemplo: $ cd ~


>9. mkdir [pasta] (cria uma pasta com o nome desejado)
Exemplo: $ mkdir programas


>10. mkdir [pasta1] [pasta2] (cria pasta1 e pasta dois ao mesmo tempo)
Exemplo: $ mkdir teste1 teste2


>11. mkdir -p [pasta]/[sub-pasta] (cria um diretório e um sub-diretório)
Exemplo: $ mkdir -p teste3/teste3_1


>12. rm -r [pasta/arquivo] (deleta uma pasta ou arquivo)
Exemplo: $ rm -r teste3


>13. mv [arquivo1] [arquivo2] (renomeia uma pasta)
Exemplo: $ mv teste teste2


>14. mv [arquivo] [caminho] (move o arquivo para um determinado caminho)
Exemplo: $ mv imagem. jpg ~/t4k_slack/Wallpapers


>15. cp [arquivo] [caminho] (copia um arquivo para um determinado caminho)
Exemplo: $ cp imagem.jpg ~/t4k_slack/Wallpapers


>16. ln -s [caminho] [link] (cria um link)
Exemplo: $ ln -s /usr/bin/limewire limewire


>17. type [executável] (busca o caminho de um executável)
Exemplo: $ type limewire


>18. cat > [arquivo] (cria novo arquivo)
Exemplo: $ cat > teste.txt


>19. cat [arquivo1] >> [arquivo2] (acrescenta arq.2 em arq.1)
Exemplo: $ cat teste1 >> teste2


>20. touch [arquivo] (cria um arquivo)
Exemplo: $ touch teste


>21. diff [arquivo1] [arquivo2] (compara os dois arquivos)
Exemplo: $ diff teste1 teste2


>22. locate [arquivo] (localiza o arquivo desejado]
Exemplo:$ locate JimiHendrix. jpg


>23. head [-linhas] [arquivo] (mostra as primeiras linhas de um arquivo)
Exemplo:$ head -10 texto.txt


>23.tail [-linhas] [arquivo] (faz exatamente o contrário do comando anterior)
Exemplo:$ tail -20 texto.txt


>24. less [arquivo] (mostra o conteúdo de um diretório)
Exemplo:$ less texto.txt


>25. more [arquivo] (mostra o conteúdo de um arquivo)
Exemplo:$ more texto.txt


>26. nl [arquivo] (mostra quantas linhas tem no arquivo)
Exemplo:$ nl texto.txt


>27. wc [arquivo] (lista número de linhas, palavras e bytes de um arquivo)
Exemplo:$ wc texto.txt


>28. [comando1] | [comando2] (conecta dois processos)
Exemplo:$ vi /etc/X11/xorg.conf | more


>29. sleep [tempo] && [comando] (executa um comando em um determinado tempo)
Exemplo:$ sleep 2 && pwd


>30. echo [mensagem] (exibe uma mensagem em seu shell)
Exemplo:$ echo Olá Big Linux


>31. alias [comando/atual] [comando_novo] (muda o nome de um comando)
Exemplo:$ alias dir=ls -l


>32. history (lista os últimos 500 comandos que você digitou)
Exemplo:$ history

>33. su (muda para o super usuário root, precisa da senha)
Exemplo:$ su, no Big Linux para ter acesso como administrador sem digitar su, digite "sudo su" sem aspas.


>34. su [usuário] (muda para outro usuário, também necessita da senha)
Exemplo:$ su fulano


>35. shutdown (reinicia o sistema)
Exemplo:$ shutdown


>36. reboot (reinicia a máquina com emergência)
Exemplo:$ reboot


>37. passwd (troca sua senha)
Exemplo:$ passwd


>38. uname (mostra o sistema operacional)
Exemplo:$ uname


>39. uname -a (mostra o sistema operacional, nome da máquina, versão do kernel e etc)
Exemplo: $ uname -a

>40. dmesg (mostra informações do sistema)
Exemplo: $ dmesg

>41. top -d [segundos] (informações detalhadas dos processos)
Exemplo: $ top -d 3

>42. ps (mostra os processos corrente "PID")
Exemplo: $ ps

>43. killall [programa] (força o término de um programa)
Exemplo: $ killall xmms

>44. xkill (transforma o ponteiro do mouse em um assassino de programa)
Exemplo:$ xkill


>45. mkfs.ext2 (formata um disquete em formato Linux)
Exemplo: $ mkfs.ext2 /dev/fd0

>46. superformat (formata um disquete em formato DOS)
Exemplo: $ superformat /dev/fd0

>47. vmstat [-tempo] (mostra a memória swap em uso)
Exemplo: $ vmstat -2

>48. arch (mostra a arquitetura do seu PC)
Exemplo: $ arch

>49. lsmod (lista os módulos da sua máquina)
Exemplo: $ lsmod

>50. insmod [módulo] (levanta um módulo forçadamente, requer root)
Exemplo: # insmod spca5x

>51. adduser (adiciona um usuário no sistema, requer root)
Exemplo:# adduser

>52. userdel [usuário] (deleta um usuário, requer root)
Exemplo: # userdel fulano

>53. userdel -r [usuário] (deleta o usuário e sua pasta que se encontra no diretório /home,
requer root)
Exemplo: # userdel -r fulano

>54. chfn [usuário] (muda informações de um usuário, requer root)
Exemplo: # chfn fulano

>55. chage -M [dias] [usuário] (expira um usuário, no dia pré-determinado, requer root)
Exemplo: # chage -M 20 fulano

>56. display [imagem.jpg] (mostra uma imagem no X, necessita do ImageMagick)
Exemplo: $ display imagem. jpg

>57. convert [imagem.png] [imagem.jpg] (converte o formato .png para . jpg, necessita
também do ImageMagick)
Exemplo: $ convert imagem.png imagem.jpg

>58. chmod (altera permissões)
Exemplo: # chmod 666 /dev/hdd

>59. mount [device] (monta um dispositivo)
Exemplo: $ mount /mnt/cdrom

>60. umount [device] (desmonta um dispositivo)
Exemplo: $ umount /mnt/cdrom

>61. eject (abre a gaveta do cd-rom)
Exemplo: $ eject /mnt/cdrom

>62. eject -t (fecha a gaveta do cdrom)
Exemplo: $ eject -t /mnt/cdrom

>63. halt (desliga o PC)
Exemplo: $ halt

>64. date (informa o dia e a hora)
Exemplo: $ date

>65. hostname (informa o nome da máquina)
Exemplo: $ hostname

>66. du [diretório] (fornece o tamanho de um diretório)
Exemplo: $ du pasta

>67. du -S [sub-diretórios] (fornece o tamanho do sub-diretório)
Exemplo: $ du -S sub_pasta

>68. [comando] & (inicia um processo em segundo plano e deixa o terminal livre para
trabalhar)
Exemplo: $ gkrellm &

>69. cal (mostra um calendário do mês atual)
Exemplo: $ cal

>70. cal [ano] (mostra os 12 meses de um determinado ano)
Exemplo: $ cal 2005

>71. last [-quantidade] (mostra informações sobre os últimos logins, onde em quantidade
você indica o número de logins)
Exemplo: $ last -10

>72. tar -zxvf[arquivo.tar.gz] (descompacta um arquivo em formato .tar.gz)
Exemplo: $ tar -zxvf amsn-0.94.tar.gz

>73. tar -jxvf [arquivo .tar.bz2] (descompacta um arquivo no formato .tar.bz2)
Exemplo: $ tar -jxvf gkrellm-0.12.tar.bz2

>74. clear (limpa a tela do shell)
Exemplo: $ clear

>75. free (mostra detalhes sobre a memória RAM)
Exemplo: $ free

>76. time [comando] (mede o tempo gasto para abrir um programa)
Exemplo: $ time amsn

>77. uptime (mostra o tempo desde do último boot)
Exemplo: $ uptime

>78. lsattr [arquivo/diretório] (lista atributos de um arquivo ou diretório)
Exemplo: $ lsattr arquivo

>79. whereis [executável/comando] (localiza o caminho de um executável/comando)
Exemplo: $ whereis amsn

>80. who (mostra quem está conectado ao sistema nesse momento)
Exemplo: $ who

>81. wget -c [URL] (faz download de arquivo na internet)
Exemplo: $ wget -c http://www.lugar.do.download/


>82. whoami (mostra quem se logou primeiro no sistema)
Exemplo: $ whoami

>83. lspci(lista os componentes PCI do seu computador)

Exemplo: $ lspci

>84. init 6 (faz reiniciar o computador mais rápido)
