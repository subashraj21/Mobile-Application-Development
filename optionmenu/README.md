# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:



## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:B Subash Raj
Registeration Number :212221040164
*/
```
## Activity_xml File:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">

<ImageView
    android:id="@+id/imageView"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:src="@drawable/amgus"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    tools:srcCompat="@tools:sample/avatars" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## OPTION XML CODE:
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
<item android:title="PRIME 1" />
<item android:title="PRIME 2" />
<item android:title="PRIME 3" />
</menu>
```
## MainActivity.java File:
```
  package com.example.menuapp;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {
 @Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
@Override
public boolean onCreateOptionsMenu(Menu menu) {
    MenuInflater m = getMenuInflater();
    m.inflate(R.menu.option,menu);
    return true;
}
}
```
## OUTPUT
![image](https://github.com/varshithathirumalachari/Mobile-Application-Development/assets/131793193/c68e3aa0-19a2-4875-8a27-128aab8d1386)

![image](https://github.com/varshithathirumalachari/Mobile-Application-Development/assets/131793193/551974ae-62e2-4365-a877-a33b43ab3b03)




## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.


