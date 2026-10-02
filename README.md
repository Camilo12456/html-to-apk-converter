# HTML to APK Converter

Este repositório é um modelo inicial para empacotar uma página HTML/CSS/JavaScript em um APK Android usando Cordova.

## O que tem aqui

- `config.xml`: configuração do aplicativo Android
- `www/`: arquivos web que serão exibidos no app
- `README.md`: instruções de uso

## Estrutura do projeto

```text
html-to-apk-converter/
├── config.xml
├── package.json
├── www/
│   ├── index.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── app.js
├── .gitignore
└── README.md
```

## Como usar

### 1) Instale as ferramentas

```bash
npm install -g cordova
```

### 2) Adicione a plataforma Android

```bash
cordova platform add android
```

### 3) Compile o APK

```bash
cordova build android
```

O APK será gerado em:

```text
platforms/android/app/build/outputs/apk/debug/app-debug.apk
```

## Personalização

Edite os arquivos em `www/` para usar seu próprio HTML, CSS e JavaScript. Caso queira acessar recursos nativos do Android (câmera, GPS, notificações, etc.), você pode adicionar plugins do Cordova.

Exemplo:

```bash
cordova plugin add cordova-plugin-camera
```

## Dica importante

Se você já tem um site em HTML e quer transformá-lo em app Android, basta copiar os arquivos da sua página para `www/` e ajustar o layout conforme necessário.

## Observação

Este é um ponto de partida para um APK. Para publicar na Play Store, será necessário assinar o APK e configurar a identidade do app.
