# PROTOCOLO BANE — pacote corrigido para usar no Lovable

## Conteúdo
- `index.html`: aplicativo original com correção final de viewport, rolagem da tela Início e posicionamento do menu inferior.
- `bane-wallpaper.png` e `splash-wallpaper.jpg`: imagens originais do app.
- `icon.png`: ícone do app.
- `manifest.json`: configuração PWA.
- `sw.js`: Service Worker corrigido, com versão de cache atualizada.

## Instrução para o Lovable
Use os arquivos deste pacote como fonte do projeto PROTOCOLO BANE. Preserve o design, as imagens, os textos, os dados, as funções e a navegação existentes. Se for necessário converter o HTML para a estrutura padrão do Lovable (React/Vite), faça uma migração fiel e mantenha todas as funcionalidades; coloque as imagens em `public/` e ajuste os caminhos dos assets.

Requisitos obrigatórios de layout: ocupar toda a altura útil do iPhone; usar `100dvh` com fallback para `100vh`; respeitar `env(safe-area-inset-top)` e `env(safe-area-inset-bottom)`; manter a barra de navegação fixa no fundo; reservar espaço para a barra no conteúdo; permitir rolagem vertical real da tela Início para que os cartões abaixo de “Evolução do peso” possam ser acessados; não deixar faixa preta vazia abaixo do app nem conteúdo escondido atrás da barra. Não aumentar artificialmente o tamanho dos cartões nem distorcer o wallpaper.

Não adicione regras CSS duplicadas no fim do arquivo para mascarar problemas. Consolide os estilos responsivos e teste em telas pequenas e grandes. Não reintroduza um Service Worker com sintaxe inválida ou cache antigo. Ao publicar alterações, atualize a versão do cache e confirme que o aplicativo abre e navega corretamente.
