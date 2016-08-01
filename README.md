# Estudos Ionic
- **[Ionic Essencial](https://github.com/jonatasleon/estudos-ionic/tree/master/ionic-essencial)**

## Comandos básicos

### Instalando Ionic
```
$ npm install -g cordova ionic
```

### Criando no projeto
```
$ ionic start <nome> [blank|sidemenu|tabs|maps|salesforce|complex-list]
```

### Executando APP no browser
```
$ ionic serve [--lab|-b|-t <android|ios>]
```

## Build Android
Para fazer a build de um APP para Android é necessário:

- ter instalado o Java JDK;
- ter instalado o Android SDK;
- fazer a atualização de pacotes no Manager Android SDK. **Desmarque** tudo que vem marcado por padrão e marque apenas:
  - Tools
    - Android SDK Tools;
    - Android SDK Platform-tools;
    - Android SDK Build-tools;
  - Android 6.0(API 23)
    - SDK Platform;
    - Google APIs;
    - Sources for Android SDK;
  - Extras
    - Android Support Library;
    - Google USB Driver;
    - Google Web Driver;
- **no windows**, adicionar a variável `ANDROID_HOME` com o valor `C:\android` (caso esse seja o path onde você instalou o Android SDK);

Então:
```
$ ionic platform add android
$ ionic build android
```

O resultado dever ser algo como:
```
BUILD SUCCESSFUL
Total time: 2 mins 57.657 secs
Built the following apk(s):
C:/workspace/app1/platforms/android/build/outputs/apk/androiddebug.apk
```
