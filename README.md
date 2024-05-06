# ADDITION-OF-TWO-NUMBERS---ANDROID-APP

## AIM:
To develop a program to create a simple app to add two numbers.

## SOFTWARE REQUIRED:
Android Studio

## ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as workshop and click Next.

Step 3: Then select the Empty Activity and click Next.

Step 4: Design layout in activity_main.xml.

Step 5: Perform the addition operation in MainActivity.java

Step 6: Save and run the application.

## PROGRAM:
```
Developed by: Sowmya V
RegisterNumber:  212222110045
```
## MainActivity.java:
```
package com.example.workshop;

import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        final EditText number1 = findViewById(R.id.editTextNumber1);
        final EditText number2 = findViewById(R.id.editTextNumber2);
        final Button addButton = findViewById(R.id.buttonAdd);
        final EditText result = findViewById(R.id.editTextResult);

        addButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                double num1 = Double.parseDouble(number1.getText().toString());
                double num2 = Double.parseDouble(number2.getText().toString());
                double sum = num1 + num2;
                result.setText(String.valueOf(sum));
            }
        });
    }
}
```
## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="16dp">

    <EditText
        android:id="@+id/editTextNumber1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter number 1"
        android:inputType="numberDecimal"/>

    <EditText
        android:id="@+id/editTextNumber2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter number 2"
        android:inputType="numberDecimal"/>

    <Button
        android:id="@+id/buttonAdd"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Add Numbers"
        android:layout_gravity="center_horizontal"/>

    <EditText
        android:id="@+id/editTextResult"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Result"
        android:focusable="false"/>

</LinearLayout>

```
## Output:
![image](https://github.com/SowmyaVisvanathan/ADDITION-OF-TWO-NUMBERS---ANDROID-APP/assets/119475775/e39312d5-6648-44d5-a2fb-d14005c50b3d)

## Result:
Thus the program to develop a simple app to add two numbers is developed successfully
