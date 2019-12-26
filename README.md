# Manual Flutter: Autenticação via SMS pelo [Firebase](https://firebase.google.com/)

Referencia: [Repositório de firebase_auth](https://github.com/FirebaseExtended/flutterfire/tree/master/packages/firebase_auth/firebase_auth)

## **Conteúdo**

1. [Passo à passo](#passo-à-passo)
2. [Aprender](#aprender)
3. [Contribuir](#contribuir)
4. [Licença](#licença)

## Passo-à-passo

#### 1. Crie um novo projeto Flutter
- Crie um novo projeto e use o codigo deste [main.dart](lib/main.dart)
![main.dart](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/main_dart.gif)

- Adicione as dependencias no pubspec.yaml
![pubspec](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/pubspec.png)

#### 2. Crie um projeto no Firebase
>Acesse o [Firebase](https://firebase.google.com/) e clique em "Primeiros passos" para acessar o [Firebase Console](https://console.firebase.google.com/)

#### 3. Registre seu projeto Flutter no seu projeto Firebase
- O nome do pacote android está em `android/app/build.gradle` na propriedade `applicationId`
- Gere a chave SHA-1

> NOTA: A utilidade `keytool` é provida pelo [Java (jdk)](https://www.oracle.com/technetwork/java/javase/downloads/index.html)

#### 4. Faça o download do arquivo de configuração





