# Script de provisionamento de servidor Apache

Este projeto contém um script em Bash para automatizar o processo de atualização de um servidor Linux e o deploy de uma aplicação web. O script realiza as seguintes ações:

1. Atualiza o sistema operacional (Ubuntu/Debian).
2. Instala o servidor web Apache.
3. Baixa e instala os arquivos de uma aplicação hospedada no GitHub.

## Requisitos

- Servidor Linux (preferencialmente Ubuntu ou Debian).
- Permissões de administrador (root) para executar os comandos de instalação e cópia de arquivos.
- Conexão com a internet para baixar pacotes e arquivos da aplicação.

## Como usar o script

1. Faça o download ou clone este repositório no servidor.
2. Conceda permissão de execução ao script:

    ```bash
    chmod +x nome_do_script.sh
    ```

3. Execute o script como root ou utilizando `sudo`:

    ```bash
    sudo ./nome_do_script.sh
    ```

## O que o script faz

- Atualiza os pacotes do sistema com `apt-get update` e `apt-get upgrade`.
- Instala o Apache2 como servidor web.
- Instala o pacote `unzip` para descompactar arquivos.
- Baixa a aplicação web de um repositório GitHub e copia os arquivos para o diretório raiz do servidor web Apache (`/var/www/html`).


