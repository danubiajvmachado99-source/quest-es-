# Simulado Formação Cidadã — projeto Android

Este projeto encapsula o HTML fornecido em uma WebView e define Android 10 (API 29) como versão mínima. O HTML original foi preservado e recebeu salvamento local de respostas, discursivas, tempo restante e estado de finalização via `localStorage`.

## Gerar o APK no Windows

1. Instale o Android Studio: https://developer.android.com/studio
2. Extraia este ZIP para uma pasta, por exemplo `C:\Projetos\SimuladoFormacaoCidada`.
3. No Android Studio, escolha **Open** e selecione a pasta extraída.
4. Aguarde a sincronização do Gradle e a instalação dos componentes solicitados.
5. No menu **Build**, escolha **Build Bundle(s) / APK(s) > Build APK(s)**.
6. O APK de depuração normalmente ficará em `app\build\outputs\apk\debug\app-debug.apk`.
7. Transfira o APK ao telefone Android 10 e permita a instalação dessa origem, se solicitado.

## Observações importantes

- Este pacote é o **projeto-fonte**, não um APK já compilado.
- O simulado abre localmente e funciona sem internet. O projeto já declara permissão de internet, mas a atualização remota do banco de questões ainda precisa de uma URL HTTPS de hospedagem e de uma integração para baixar/validar a versão remota. Não configure uma URL desconhecida como fonte de código.
- O salvamento usa o armazenamento local da WebView no mesmo aparelho. Limpar os dados do aplicativo pode apagar o progresso.
- A nota automática das discursivas é aproximada, conforme o HTML original.
