# Demo-My-Map-Maui

**Get a Google Maps API key**
To use the [Map](https://learn.microsoft.com/en-us/dotnet/api/microsoft.maui.controls.maps.map) control on Android you must generate an API key, which will be consumed by the Google Maps SDK on which the Map control relies on Android. To do this, follow the instructions in Set up in the Google Cloud Console and Use API Keys on developers.google.com.

Once you've obtained an API key it must be added within the <application> element of your Platforms/Android/AndroidManifest.xml file, by specifying it as the value of the com.google.android.geo.API_KEY metadata:

 
<application android:allowBackup="true" android:icon="@mipmap/appicon" android:roundIcon="@mipmap/appicon_round" android:supportsRtl="true">
  <meta-data android:name="com.google.android.geo.API_KEY" android:value="PASTE-YOUR-API-KEY-HERE" />
</application>
  
  
This embeds the API key into the manifest. Without a valid API key the Map control will display a blank grid.

 
