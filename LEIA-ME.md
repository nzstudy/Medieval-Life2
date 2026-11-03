# Medieval Life: gerar o APK
Opção A (sem instalar nada): crie um repositório no GitHub, envie estes arquivos, abra a aba Actions > "Build APK" > Run workflow. Ao terminar, baixe `medieval-life-apk` (contém app-debug.apk).
Opção B (local, com Node 20, JDK 17 e Android SDK): npm install && npx cap add android && npx cap sync android && cd android && ./gradlew assembleDebug
O APK sai em android/app/build/outputs/apk/debug/. Para instalar, permita "fontes desconhecidas" no celular.
Para atualizar o jogo, troque www/index.html. A fonte do Google precisa de internet; sem ela o jogo usa Georgia.
