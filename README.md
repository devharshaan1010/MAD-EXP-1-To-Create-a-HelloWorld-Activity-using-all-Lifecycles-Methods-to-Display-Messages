# MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages

## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Studio and then click on File -> New -> New project.

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
Developed by: S DEV HARSHAAN
Registration Number : 212221040035
*/
```
activity_main.xml :
```
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</android.support.constraint.ConstraintLayout>
```
MainActivity.java :
```
package com.example.exp1;
import android.os.Bundle;
import android.support.v7.app.AppCompatActivity;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast.makeText(this, "onCreate Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onRestart(){
        Toast.makeText(this, "onRestart Called", Toast.LENGTH_SHORT).show();
        super.onRestart();
    }
    @Override
    protected void onStart(){
        Toast.makeText(this, "onStart Called", Toast.LENGTH_SHORT).show();

        super.onStart();
    }
    @Override
    protected void onResume(){
        Toast.makeText(this, "onResume Called", Toast.LENGTH_SHORT).show();

        super.onResume();
    }
    @Override
    protected void onPause(){
        Toast.makeText(this, "onPause Called", Toast.LENGTH_SHORT).show();

        super.onPause();
    }
    @Override
    protected void onStop(){
        Toast.makeText(this, "onStop Called", Toast.LENGTH_SHORT).show();

        super.onStop();
    }
    @Override
    protected void onDestroy(){
        Toast.makeText(this, "onDestroy Called", Toast.LENGTH_SHORT).show();

        super.onDestroy();
    }
}
```
## OUTPUT:

![image](https://github.com/Siddarthan999/MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages/assets/91734840/9a1f954e-a9c8-4cbf-bf73-6edbb97df378)

![image](https://github.com/Siddarthan999/MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages/assets/91734840/a2ef3eb2-8b95-4377-be72-e80599e17685)

![image](https://github.com/Siddarthan999/MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages/assets/91734840/abe0f11a-98de-4e73-8fa9-67074ed1aa8e)

![image](https://github.com/Siddarthan999/MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages/assets/91734840/dabf2256-c354-4173-839e-25a6f448f5b2)

![image](https://github.com/Siddarthan999/MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages/assets/91734840/9d96a188-d996-40e2-b21d-7dfd5ffc26cd)

![image](https://github.com/Siddarthan999/MAD-EXP-1-To-Create-a-HelloWorld-Activity-using-all-Lifecycles-Methods-to-Display-Messages/assets/91734840/6f3771ca-4c08-485a-973c-bd0cc782ad32)

## RESULT:
Thus, a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
