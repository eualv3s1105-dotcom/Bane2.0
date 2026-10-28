# PROTOCOLO BANE — GitHub Pages

Este pacote contém os arquivos estáticos do aplicativo, preparados para publicação pelo GitHub Pages.

## Publicar
1. Abra o repositório GitHub onde deseja hospedar o aplicativo.
2. Carregue **todos os arquivos desta pasta diretamente na raiz do repositório** (não envie uma pasta externa contendo os arquivos).
3. Faça commit das alterações na branch configurada para o GitHub Pages.
4. Em **Settings → Pages**, selecione a branch e a pasta correta (`/(root)` se os arquivos estiverem na raiz) e salve.
5. Aguarde a publicação e abra o endereço `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

## Notas
- `index.html`, `manifest.json`, `sw.js` e as imagens precisam permanecer juntos na mesma pasta.
- O caminho do Service Worker é relativo para suportar repositórios publicados em subcaminhos do GitHub Pages.
- O arquivo `.nojekyll` evita que o GitHub Pages processe os arquivos estáticos pelo Jekyll.
- Após publicar uma atualização, feche e reabra o Safari. Se continuar aparecendo uma versão antiga, remova o atalho antigo da Tela de Início e abra novamente o endereço publicado; o cache pode levar um momento para atualizar.
- O pacote foi preparado para hospedagem estática. A aparência e o funcionamento final devem ser conferidos no Safari após a publicação.
