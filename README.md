# Title
get-JSON-data-using-API-and-store-SQLITE
# Description
It's a sample project to get JSON data from web using API and store it sqlite database using content provider.Also here show how to share data in many platform.Also use share Preference.
# Usages 
### Build.gradle(app)
````````
 implementation 'com.android.support:recyclerview-v7:26.1.0'
    implementation 'com.android.support:preference-v7:26.1.0'
````````
### Mainfest.xml
``````````
<!-- This permission is necessary in order for Sunshine to perform network access. -->
    <uses-permission android:name="android.permission.INTERNET"/>
    
     <!-- Our ContentProvider -->
        <provider
            android:name=".data.WeatherProvider"
            android:authorities="@string/content_authority"
            android:exported="false"/>
``````````
