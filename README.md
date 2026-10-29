# ShoyoRender

Renderizador do SHOYO LAUNCHER para o Minecraft **1.8.9**.

Ele e um fork do **GL4ES** (traduz OpenGL antigo para OpenGL ES), licenca **MIT**,
copyright Sebastien Chevalier e Ryan Hileman. Os avisos de copyright e a licenca
originais ficam no arquivo `LICENSE-GL4ES` e nao podem ser removidos.

Versao 0.1: mesmo comportamento do GL4ES, so compilado por nos e com o nome ShoyoRender.
Os ajustes para o 1.8.9 entram como arquivos em `patches/` (aplicados em ordem na compilacao).

## Como compila
O GitHub Actions baixa o GL4ES (commit fixo em `GL4ES_COMMIT`), aplica `patches/*.patch`,
compila com o Android NDK (arm64-v8a) e publica o artefato `ShoyoRender` com `libshoyorender.so`.

Baixar: `gh run download -n ShoyoRender -D out`
