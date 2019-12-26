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

![create firebase project](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/create_firebase_project.gif)

#### 3. Registre seu projeto Flutter no seu projeto Firebase
- O nome do pacote android está em `android/app/build.gradle` na propriedade `applicationId`

![applicationId](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/applicationId.gif)

- Gere a chave SHA-1 pelo terminal

![SHA-1](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/sha1.gif)

> NOTA: A utilidade `keytool` é provida pelo [Java (jdk)](https://www.oracle.com/technetwork/java/javase/downloads/index.html)

#### 4. Faça o download do arquivo de configuração
Coloque o arquivo de configuração `google-services.json` em `android/app`
![google-services.json](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/google_json_file.gif)

## collapsible markdown?

<details><summary>CLICK ME</summary>
<p>

#### yes, even hidden code blocks!

![](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/google_json_file.gif)
![](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/google_json_file.gif)
![](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/google_json_file.gif)

</p>
</details>


