# Pequeno Habitante — Android wrapper

Este projeto empacota o protótipo web original dentro de uma WebView Android.
Os arquivos HTML, CSS e JavaScript ficam em `app/src/main/assets/`.

## Gerar o APK pelo GitHub Actions (sem instalar Android Studio)

1. Crie um repositório no GitHub e envie todos os arquivos desta pasta.
2. Abra a aba **Actions** do repositório.
3. Se solicitado, habilite workflows.
4. Selecione **Build Pequeno Habitante APK** e clique em **Run workflow**.
5. Quando terminar, abra a execução concluída e baixe o artefato **Pequeno-Habitante-APK**.
6. Extraia o ZIP do artefato: dentro estará `app-debug.apk`.
7. Envie o APK ao celular e abra-o para instalar. O Android pode pedir autorização para instalar apps dessa origem.

## Editar o bichinho depois

- Perguntas, falas, personagem e comportamento: `app/src/main/assets/main.js`
- Aparência e layout: `app/src/main/assets/style.css`
- Estrutura da tela: `app/src/main/assets/index.html`

A versão de teste usa armazenamento local da WebView. O nome e o diário ficam salvos no aparelho.
O APK gerado pelo workflow é de depuração (`debug`), adequado para teste pessoal.
