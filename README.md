# Manual Flutter: Autenticação via SMS pelo [Firebase](https://firebase.google.com/)

Referencia: [Repositório de firebase_auth](https://github.com/FirebaseExtended/flutterfire/tree/master/packages/firebase_auth/firebase_auth)

## **Conteúdo**

1. [Passo à passo](#passo-à-passo)
2. [Aprender](#aprender)
3. [Contribuir](#contribuir)
4. [Licença](#licença)

## Passo-à-passo
Vejá também o [passo à passo simplificado](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/README.md)

#### 1. Crie um novo projeto Flutter
- Crie um novo projeto e use o codigo deste [main.dart](lib/main.dart)

![main.dart](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/main_dart.gif)

- Adicione as dependencias no pubspec.yaml
  - google_sign_in: ^4.0.0
  - firebase_core: ^0.4.0+8
  - firebase_dynamic_links: ^0.3.0
  - uuid: ^2.0.2
  - firebase_auth: ^0.15.3
  
![pubspec](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/pubspec.png)

----------------

#### 2. Crie um projeto no Firebase
Acesse o [Firebase](https://firebase.google.com/) e clique em "Primeiros passos" para acessar o [Firebase Console](https://console.firebase.google.com/)

Adicione um novo projeto no firebase. Defina nome do novo projeto usando o nome do seu projeto
do Android Studio que está registrado no cabeçalho do [pubspec.yaml](pubspec.yaml). Em seguida permita o uso do 
Google Analytics e então estára sendo criado o novo projeto no Firebase. 

![create firebase project](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/create_firebase_project.gif)

----------------

#### 3. Registre seu projeto Flutter no seu projeto Firebase
- Preencha o campo "Nome do pacote do Android" com o nome do pacote android do projeto Flutter, que está em `android/app/build.gradle` na propriedade `applicationId`.  

![applicationId](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/applicationId.gif)

- Para gerar a [chave SHA-1](https://developers.google.com/android/guides/client-auth) pelo terminal
, utilize o terminal para executar o comando:
```
Mac/Linux:
keytool -list -v \
-alias androiddebugkey -keystore ~/.android/debug.keystore

Windows:
keytool -list -v \
-alias androiddebugkey -keystore %USERPROFILE%\.android\debug.keystore
```

![SHA-1](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/sha1.gif)

> NOTA: A utilidade `keytool` é provida pelo [Java (jdk)](https://www.oracle.com/technetwork/java/javase/downloads/index.html)

----------------

#### 4. Faça o download do arquivo de configuração
Nesta etapa o Firebase disponibilizará o arquivo `google-services.json` para download. Coloque este arquivo de configuração na pasta `android/app`.

![google-services.json](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/google_json_file.gif)

----------------

#### 5. Adicione o SDK do Firebase
Nesta etapa, verifique se as linhas especificadas pelo Firebase estão nos arquivos `build.gradle` dos diretórios `android` e `android/app`. 
> NOTA: Já que voce está configurando os arquivos gradle, atualize as dependencias desatualizadas, o Android Studio realça as versões desatualizadas. 


- Adicione as linhas especificadas pelo guia do Firebase em `<projeto>/android/build.gradle`

![android/build.gradle](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/firebase_sdk_android.gif)

- Adicione as linhas especificadas pelo guia do Firebase em `<projeto>/android/app/build.gradle`

![android/build.gradle](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/firebase_sdk_android_app.gif)

----------------

#### 6. Execute o app para testar a conexão com o Firebase

O ultimo passo de registrar o app Flutter no Firebase é executando o Flutter run. Após a compilação, o Firebase reconhecerá a conexão e finalizará a seção de registro.

![Execute App](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/run_app.gif)

----------------

#### 7. Habilite a autenticação por smartphone

No menu esquerdo, acesse Desenvolver->**Authentication**. Em Authentication, selecione a aba **Método de login**. Na lista de provedores de login, clique em **Smartphone** e ative-o.

![Enable phone auth](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/enable_phone_auth.gif)

----------------

#### 8. Execute o app e teste a autenticação por SMS

Agora só resta testar o app para receber seu SMS de autenticação

<img src="https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/running_app.gif" width="200">

## **Aprender**

[firebase-phone-auth-with-flutter](https://medium.com/@fayaz07/firebase-phone-auth-with-flutter-db7e934ef46f)

[pub.dev/packages/firebase_auth](https://pub.dev/packages/firebase_auth)

[github.com/FirebaseExtended/flutterfire](https://github.com/FirebaseExtended/flutterfire)

[firebase.google.com/docs](https://firebase.google.com/docs)


## **Contribuir**

Contribuições são sempre muito bem vindas! Não precisam ser somente através de desenvolvimento de código, qualquer ajuda com ideias, sugestões, melhorias na documentação e doações são sempre muito apreciadas!

Participe da comunidade [Projeto que Vale](http://www.projetoquevale.com.br/) e colabore da forma que achar melhor.


## **Licença**

MIT License

Copyright (c) 2019 PROJETO QUE VALE

É concedida permissão, gratuitamente, a qualquer pessoa que obtenha uma cópia deste software e dos arquivos de documentação associados (o "Software"), para negociar o Software sem restrições, incluindo, sem limitação, os direitos de uso, cópia, modificação e fusão , publicar, distribuir, sublicenciar e / ou vender cópias do Software, e permitir que as pessoas a quem o Software é fornecido o façam, sujeitas às seguintes condições:

O aviso de copyright acima e este aviso de permissão devem ser incluídos em todas as cópias ou partes substanciais do Software.

O SOFTWARE É FORNECIDO "NO ESTADO EM QUE SE ENCONTRA", SEM NENHUM TIPO DE GARANTIA, EXPRESSA OU IMPLÍCITA, INCLUINDO, MAS NÃO SE LIMITANDO ÀS GARANTIAS DE COMERCIALIZAÇÃO, ADEQUAÇÃO A UM FIM ESPECÍFICO E NÃO VIOLAÇÃO. EM NENHUMA CIRCUNSTÂNCIA, OS AUTORES OU PROPRIETÁRIOS DE DIREITOS DE AUTOR PODERÃO SER RESPONSABILIZADOS POR QUAISQUER REIVINDICAÇÕES, DANOS OU OUTRAS RESPONSABILIDADES, QUER EM ACÇÃO DE CONTRATO, DELITO OU DE OUTRA FORMA, DECORRENTES DE, OU EM CONEXÃO COM O SOFTWARE OU O USO OU OUTRAS NEGOCIAÇÕES NO PROGRAMAS.


