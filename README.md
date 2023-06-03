# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


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
Program to print the text “Hello World”.
Developed by:Golla Navya
Registeration Number :212221040048
*/
```
## activity_main.xml:
```
activity_main.xml:
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 tools:context=".MainActivty">
 <TextView
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:text="Hello World!"
 app:layout_constraintBottom_toBottomOf="parent"
 app:layout_constraintEnd_toEndOf="parent"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## PROGRAM:
```
package com.example.life;
import android.content.Context;
import android.content.Intent;
import android.support.annotation.Nullable;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_main);
       Toast.makeText(this, "onCreate Called",
Toast.LENGTH_SHORT).show();
 }
 
 @Override
 protected void onRestart() {
      Toast.makeText(this, "onRestart Called",
Toast.LENGTH_SHORT).show();
 super.onRestart();
 }
 
 @Override
 protected void onStart() {
      Toast.makeText(this, "onStart Called",
Toast.LENGTH_SHORT).show();
 super.onStart();
 }
 
 @Override
 protected void onResume() {
 Toast.makeText(this, "onResume Called",
Toast.LENGTH_SHORT).show();
 super.onResume();
 }
 
 @Override
 protected void onPause() {
      Toast.makeText(this, "onPause Called",
Toast.LENGTH_SHORT).show();
 super.onPause();
 }
 
 @Override
 protected void onStop() {
      Toast.makeText(this, "onStop Called",
Toast.LENGTH_SHORT).show();
 super.onStop();
 }
 
 @Override
 protected void onDestroy() {
      Toast.makeText(this, "onDestroy Called",
Toast.LENGTH_SHORT).show();
 super.onDestroy();
 }}
```

## OUTPUT
![Screenshot (37)](https://github.com/gsuryanavya/lifecycle/assets/133086963/e20cec45-abfb-4cca-b883-01fe573b83bf)
![Screenshot (38)](https://github.com/gsuryanavya/lifecycle/assets/133086963/3767a7dd-6d71-44e3-9936-81936d28497d)
![Screenshot (39)](https://github.com/gsuryanavya/lifecycle/assets/133086963/7c4524a1-4a1e-464e-a72e-9ece54e765fc)
![Screenshot (40)](https://github.com/gsuryanavya/lifecycle/assets/133086963/20319a4c-9ebe-4067-b0b0-ce8852dbab00)
![Screenshot (44)](https://github.com/gsuryanavya/lifecycle/assets/133086963/e237b1ce-1406-46ba-87fb-3950848ed0d1)
![Screenshot (45)](https://github.com/gsuryanavya/lifecycle/assets/133086963/889b187f-ada9-4085-a0f0-0db2727a4c7c)
![Screenshot (46)](https://github.com/gsuryanavya/lifecycle/assets/133086963/9b2e85b5-ac54-4fb3-bcbb-7982b1a49506)




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
