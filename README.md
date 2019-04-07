# LayoutTest
实验二：布局实验

![](https://github.com/wowoHead/LayoutTest/blob/master/%E5%AE%9E%E9%AA%8C%E4%BA%8C/%E4%B8%BB%E7%95%8C%E9%9D%A2.png)

```

package com.example.ssh.layouttest;

import android.content.Intent;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button btn1 = (Button)findViewById(R.id.btn1);
        btn1.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent(MainActivity.this,Main2Activity.class);
                startActivity(intent);
            }
        });

        Button btn2 = (Button)findViewById(R.id.btn2);
        btn2.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent(MainActivity.this,Main3Activity.class);
                startActivity(intent);
            }
        });

        Button btn3 = (Button)findViewById(R.id.btn3);
        btn3.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent(MainActivity.this,Main4Activity.class);
                startActivity(intent);
            }
        });

    }
}

<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:orientation="vertical"    >

        <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content">
        <Button
            android:id="@+id/btn1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="LinearLayout"/>
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
            <Button
                android:id="@+id/btn2"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="ConstraintLayout"/>
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
            <Button
                android:id="@+id/btn3"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="TableLayout"/>
        </LinearLayout>

</LinearLayout>



</android.support.constraint.ConstraintLayout>

```


实验二LinearLayout

![](https://github.com/wowoHead/LayoutTest/blob/master/%E5%AE%9E%E9%AA%8C%E4%BA%8C/LinearLayout.png)

```

<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".Main2Activity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:orientation="horizontal">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="One.one"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="One.two"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="One.three"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="One.four"/>

        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:orientation="horizontal">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Two.one"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Two.two"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Two.three"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Two.four"/>

        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:orientation="horizontal">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Three.one"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Three.two"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Three.three"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Three.four"/>

        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:orientation="horizontal">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Four.one"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Four.two"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Four.three"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:text="Four.four"/>

        </LinearLayout>

    </LinearLayout>

</android.support.constraint.ConstraintLayout>

```

实验二ConstraintLayout

![](https://github.com/wowoHead/LayoutTest/blob/master/%E5%AE%9E%E9%AA%8C%E4%BA%8C/ConstraintLayout.png)

```

<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".Main3Activity">


    <TextView
        android:id="@+id/textView"
        android:layout_width="89dp"
        android:layout_height="53dp"
        android:layout_marginStart="16dp"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="8dp"
        android:layout_marginBottom="8dp"
        android:background="#ffffff"
        android:text="white"
        android:textAlignment="center"
        android:textSize="20dp"
        app:layout_constraintBottom_toTopOf="@+id/textView4"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.019" />

    <TextView
        android:id="@+id/textView2"
        android:layout_width="88dp"
        android:layout_height="51dp"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginRight="8dp"
        android:background="#000eee"
        android:text="blue"
        android:textAlignment="center"
        android:textSize="25dp"
        app:layout_constraintEnd_toStartOf="@+id/textView3"
        app:layout_constraintStart_toEndOf="@+id/textView"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="88dp"
        android:layout_height="55dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="16dp"
        android:layout_marginRight="16dp"
        android:layout_marginBottom="8dp"
        android:text="green"
        android:textAlignment="center"
        android:textSize="25dp"
        android:background="#f0f0"
        app:layout_constraintBottom_toTopOf="@+id/textView5"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.0" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="100dp"
        android:layout_height="118dp"
        android:layout_marginStart="24dp"
        android:layout_marginLeft="24dp"
        android:layout_marginBottom="116dp"
        android:text="indigo"
        android:background="#e0e0e0"
        android:textAlignment="center"
        android:textSize="25dp"
        app:layout_constraintBottom_toTopOf="@+id/textView7"
        app:layout_constraintStart_toStartOf="parent" />

    <TextView
        android:id="@+id/textView5"
        android:layout_width="100dp"
        android:layout_height="116dp"
        android:layout_marginEnd="16dp"
        android:layout_marginRight="16dp"
        android:layout_marginBottom="116dp"
        android:text="violet"
        android:textAlignment="center"
        android:textSize="25dp"
        android:background="#e0e"
        app:layout_constraintBottom_toTopOf="@+id/textView7"
        app:layout_constraintEnd_toEndOf="parent" />

    <TextView
        android:id="@+id/textView6"
        android:layout_width="100dp"
        android:layout_height="118dp"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginRight="8dp"
        android:layout_marginBottom="8dp"
        android:text="yellow"
        android:background="#eee000"
        android:textAlignment="center"
        android:textSize="25dp"
        app:layout_constraintBottom_toTopOf="@+id/textView7"
        app:layout_constraintEnd_toStartOf="@+id/textView5"
        app:layout_constraintStart_toEndOf="@+id/textView4"
        app:layout_constraintTop_toBottomOf="@+id/textView2" />

    <TextView
        android:id="@+id/textView7"
        android:layout_width="380dp"
        android:layout_height="107dp"
        android:layout_marginEnd="8dp"
        android:layout_marginRight="8dp"
        android:layout_marginBottom="8dp"
        android:text="black"
        android:background="#000000"
        android:textAlignment="center"
        android:textSize="25dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />
</android.support.constraint.ConstraintLayout>

```

实验二TableLayout

![](https://github.com/wowoHead/LayoutTest/blob/master/%E5%AE%9E%E9%AA%8C%E4%BA%8C/TableLayout.png)

```

<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".Main4Activity">

    <TableRow
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="1">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Open..."
            android:textSize="20dp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Ctrl+O"
            android:textSize="20dp"
            android:gravity="end" />

    </TableRow>

    <TableRow
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="1">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Save..."
            android:textSize="20dp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Ctrl+S"
            android:textSize="20dp"
            android:gravity="end" />

    </TableRow>

    <TableRow
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="1">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Save As..."
            android:textSize="20dp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Ctrl+Shift+S"
            android:textSize="20dp"
            android:gravity="end" />

    </TableRow>

    <TableRow
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="1">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="X Import..."
            android:textSize="20dp"/>


    </TableRow>

    <TableRow
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="1">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="X Export..."
            android:textSize="20dp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Ctrl+E"
            android:textSize="20dp"
            android:gravity="end" />

    </TableRow>

    <TableRow
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="20">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="Quit"
            android:textSize="20dp"/>


    </TableRow>

</TableLayout>

```
