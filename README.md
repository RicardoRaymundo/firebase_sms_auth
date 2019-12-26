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

<details><summary>main.dart</summary>
<p>

![main.dart](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/main_dart.gif)


</p>
</details>

- Adicione as dependencias no pubspec.yaml

<details><summary>pubspeck.yaml</summary>
<p>

![pubspec](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/pubspec.png)


</p>
</details>

#### 2. Crie um projeto no Firebase
Acesse o [Firebase](https://firebase.google.com/) e clique em "Primeiros passos" para acessar o [Firebase Console](https://console.firebase.google.com/)

<details><summary>Criando projeto no Firebase</summary>
<p>

![create firebase project](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/create_firebase_project.gif)


</p>
</details>

#### 3. Registre seu projeto Flutter no seu projeto Firebase
- O nome do pacote android está em `android/app/build.gradle` na propriedade `applicationId`

<details><summary>Registrando a applicationId</summary>
<p>

![applicationId](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/applicationId.gif)


</p>
</details>

- [Gere a chave SHA-1](https://developers.google.com/android/guides/client-auth) pelo terminal

<details><summary>Gerando chave SHA-1</summary>
<p>

![SHA-1](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/sha1.gif)


</p>
</details>

> NOTA: A utilidade `keytool` é provida pelo [Java (jdk)](https://www.oracle.com/technetwork/java/javase/downloads/index.html)

#### 4. Faça o download do arquivo de configuração
Coloque o arquivo de configuração `google-services.json` em `android/app`

<details><summary>Colocando o arquivo do google em `android/app`</summary>
<p>

![google-services.json](https://github.com/RicardoRaymundo/firebase_sms_auth/blob/master/images%26gifs/google_json_file.gif)


</p>
</details>


#### 4. Adicione o SDK do Firebase
Adicione as linhas especificadas pelo guia do Firebase em `<projeto>/android/build.gradle`


Adicione as linhas especificadas pelo guia do Firebase em `<projeto>/android/app/build.gradle`





