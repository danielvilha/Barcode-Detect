# Barcode Detect

* Language: Java
* Platform: Android

O último lançamento do SDK de Google Play Services inclui a mobile vision API, que entre outras coisas, torna muito fácil criar aplicativos capazes de detectar e ler códigos QR em tempo real. Neste aplicativo tem um exemplo prático de como usar essa API.

## Example

![](/Screenshots/Screenshot_1.png) ![](/Screenshots/Screenshot_2.png)

## Requirements

Pode ser usado em qualquer vesão do Android, porém no projeto eu utilizei as versões:
- Android 5.1+
- AndroidStudio 3.0


## Usage

1. Adicionar permissão de câmera e dependência no AndroidManifest.xml
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"

    ...

    <uses-permission android:name="android.permission.CAMERA" />

    <application

        ...

        <meta-data android:name="com.google.android.gms.vision.DEPENDENCIES" android:value="barcode"/>
    </application>

</manifest>
```

2. Adicionar a dpeendência do play-services no app build.grade
```
dependencies {

    ...

    implementation 'com.google.android.gms:play-services:11.6.0'

    ...

}
```

## Documentation
A documentação completa está disponível em [Barcode API Overview](https://developers.google.com/vision/android/barcodes-overview).<br/>
Google exemplo [Barcode Detection with the Mobile Vision API](https://codelabs.developers.google.com/codelabs/bar-codes/#0).

## Author

Daniel Vilha