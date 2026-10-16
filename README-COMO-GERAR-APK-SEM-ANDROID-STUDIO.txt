COMO GERAR O APK SEM INSTALAR ANDROID STUDIO

Este projeto já inclui um fluxo do GitHub Actions para compilar o APK na nuvem.

1. Entre em https://github.com/ e crie uma conta, se ainda não tiver.
2. Crie um repositório novo. Para manter o código privado, escolha Private.
3. Descompacte este ZIP no computador.
4. Envie todos os arquivos e pastas que estão dentro de SimuladoFormacaoCidadaAndroid para o repositório do GitHub. Não envie a pasta externa que contém tudo; envie o conteúdo dela, incluindo a pasta oculta .github.
   Dica: no GitHub, use Add file > Upload files e arraste os arquivos. Confira se a pasta .github/workflows/gerar-apk.yml foi enviada.
5. Abra a aba Actions do repositório.
6. Se aparecer um aviso para habilitar workflows, clique para habilitar.
7. Selecione "Gerar APK do Simulado" e clique em Run workflow > Run workflow.
   O fluxo também inicia automaticamente quando você envia alterações para a branch main ou master.
8. Aguarde a execução terminar com marca verde. Abra a execução e, em Artifacts, clique em SimuladoFormacaoCidada-APK para baixar um ZIP.
9. Extraia o ZIP baixado. Dentro estará app-debug.apk.
10. Passe o APK para o celular Android 10 ou superior e abra-o para instalar. Se o Android pedir, permita a instalação de apps dessa fonte nas configurações.

IMPORTANTE
- Este método compila na nuvem; não instala Android Studio no seu computador.
- O APK de depuração é adequado para teste/uso pessoal, não é uma versão de publicação assinada para a Play Store.
- O arquivo gerado fica disponível no GitHub Actions por 14 dias.
- O projeto atual salva o progresso localmente no aparelho. Atualização automática de perguntas online ainda precisa ser configurada separadamente.
- Se a compilação falhar, abra a execução no GitHub Actions e copie as últimas linhas do erro para pedir ajuda.
