# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”
Developed by : SELVAMUTHU KUMARAN V
Registeration Number : 212222040151
*/
```
## MAIN ACTIVITY JAVA:
```
package com.example.steve;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();

    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onstart Called", Toast.LENGTH_LONG);
        toast.show();

    }

    @Override
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }

    @Override
    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "OnStop called", Toast.LENGTH_LONG);
        toast.show();
    }

    @Override
    protected void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "OnDestroy called", Toast.LENGTH_LONG);
        toast.show();
    }

}
```
## XML:
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@drawable/ic_launcher_foreground"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.Steve"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>

```
## OUTPUT
![Screenshot 2024-03-09 112014](https://github.com/selva258963/lifecyclemethods/assets/121961701/4c3dae8f-d13d-4759-a158-101763bad55c)
![image](https://github.com/selva258963/lifecyclemethods/assets/121961701/4abf943f-663d-48d8-8f26-23c89e63e34a)
![image](https://github.com/selva258963/lifecyclemethods/assets/121961701/158c079b-fa12-4011-93cf-422d6bd78a5e)
![image](https://github.com/selva258963/lifecyclemethods/assets/121961701/2b6f98bc-0053-4927-bfe7-57bfa1e79348)
![image](https://github.com/selva258963/lifecyclemethods/assets/121961701/6d8f0b62-1e3e-425c-9091-cc4340537be4)
![Screenshot 2024-03-09 111835](https://github.com/selva258963/lifecyclemethods/assets/121961701/f1a4de5b-ec54-4017-8eaf-2ed57b9ffb04)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
