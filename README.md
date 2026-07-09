# Tom Music

Bot de música para Discord, focado em simplicidade, agilidade e uma experiência direta para tocar áudio do YouTube no seu servidor.

## Destaques

- Reprodução de músicas via URL do YouTube
- Comandos simples para tocar, pausar, retomar e parar a reprodução
- Estrutura enxuta, fácil de entender e evoluir
- Uso de variáveis de ambiente para proteger o token do bot

## Funcionalidades

- `&play <url>`: conecta ao canal de voz e toca o áudio do link informado
- `&pause`: pausa a música atual
- `&resume`: retoma a reprodução
- `&stop`: para a música e desconecta o bot

## Requisitos

Antes de executar o projeto, você vai precisar de:

- Python 3.10 ou superior
- Um bot criado no Discord Developer Portal
- `ffmpeg` instalado na máquina
- Dependências Python do projeto

## Instalação

1. Clone o repositório.
2. Crie e ative um ambiente virtual, se quiser isolar as dependências.
3. Instale os pacotes necessários.
4. Crie um arquivo `.env` na raiz do projeto com o token do bot.

Exemplo de `.env`:

```env
discord_token=SEU_TOKEN_AQUI
```

## Execução

O ponto de entrada principal é o arquivo `main.py`.

```bash
python main.py
```

## Estrutura do projeto

- `main.py`: inicia a aplicação
- `tom_music.py`: contém a lógica do bot e os comandos
- `.env`: armazena o token do Discord de forma segura
- `venv/`: ambiente virtual local, caso você esteja usando um

## Como usar

Depois de iniciar o bot e adicioná-lo ao seu servidor:

1. Entre em um canal de voz.
2. Envie `&play <url>` com um link válido do YouTube.
3. Use `&pause`, `&resume` e `&stop` conforme necessário.

## Evolução do projeto

Este projeto ainda está em evolução e já foi pensado para crescer além do YouTube. Algumas ideias para próximas versões:

- Suporte a mais plataformas de música
- Botões de interação para facilitar o controle
- Melhorias de estabilidade e experiência de uso

## Observações

O projeto utiliza `yt-dlp` para extrair o áudio e `ffmpeg` para a reprodução. Se o bot não tocar corretamente, o primeiro ponto a verificar costuma ser a instalação do `ffmpeg` e a configuração do token no `.env`.

## Contribuição

Sugestões, melhorias e novas funções são bem-vindas. O objetivo é transformar o Tom Music em um bot cada vez mais útil, leve e fácil de manter.
