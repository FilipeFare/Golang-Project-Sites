🕵️ Monitoramento de Sites em Go

Este é um simples programa escrito em Go para monitorar a disponibilidade de sites. Ele realiza requisições HTTP, verifica se os sites estão online, armazena os resultados em logs e exibe esses logs quando solicitado.

📋 Funcionalidades

    Monitoramento de sites via HTTP GET

    Registro de status de disponibilidade em um arquivo de log

    Leitura de sites a serem monitorados a partir de um arquivo de texto (sites.txt)

    Exibição dos logs de monitoramento

    Menu interativo no terminal

🚀 Como usar
Pré-requisitos

    Go instalado (versão 1.18 ou superior recomendada)

Passo a passo

    Clone este repositório ou copie os arquivos para o seu ambiente local.

    Crie um arquivo chamado sites.txt na mesma pasta que o programa, com os sites que deseja monitorar, um por linha. Exemplo:

https://www.google.com
https://www.youtube.com
https://www.alura.com.br

    Compile o programa:

go build ProjetoCompleto.go

Menu interativo

Ao iniciar, o programa mostrará um menu com as seguintes opções:

1 - Iniciar Monitoramento
2 - Exibir Logs
0 - Sair do Programa

📁 Arquivos importantes

    sites.txt - Contém a lista de sites a serem monitorados.

    log.txt - Armazena o histórico de logs dos testes de disponibilidade.

🧠 Como funciona

    O programa faz 5 rodadas de monitoramento, com intervalos de 5 segundos entre elas.

    A cada teste, ele verifica se o site responde com código 200 OK.

    Cada resultado (online ou offline) é salvo no arquivo log.txt com data e hora.

🛠️ Tecnologias

    Linguagem: Go

    Pacotes usados: net/http, os, bufio, strings, strconv, time

✍️ Autor

    FilipeFare



