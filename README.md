# Barcode-Detect

## Example

![](/Screenshots/Screenshot_1.png) ![](/Screenshots/Screenshot_2.png)

## Requirements
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
Full documentation is available on [Barcode API Overview](https://developers.google.com/vision/android/barcodes-overview).<br/>
Google example [Barcode Detection with the Mobile Vision API](https://codelabs.developers.google.com/codelabs/bar-codes/#0).

## Author

Daniel Vilha