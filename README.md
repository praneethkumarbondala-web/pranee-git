# pranee-git

my info
this is about my personal information





/ ========================= // 1. LoginActivity.java // ========================= package com.example.goldjarapp;

import android.content.Intent; import android.os.Bundle; import android.view.View; import android.widget.Button; import android.widget.EditText; import androidx.appcompat.app.AppCompatActivity;

public class LoginActivity extends AppCompatActivity {

EditText username, password; Button loginBtn; @Override protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity\_login); username = findViewById(R.id.username); password = findViewById(R.id.password); loginBtn = findViewById(R.id.loginBtn); loginBtn.setOnClickListener(v -> { // Simple validation if(username.getText().toString().equals("member1") \&\& password.getText().toString().equals("1234")) { Intent intent = new Intent(LoginActivity.this, HomeActivity.class); startActivity(intent); } }); }

}

// ========================= // activity\_login.xml // ========================= /\*

<EditText android:id="@+id/username" android:hint="Username" android:layout\_width="match\_parent" android:layout\_height="wrap\_content" /> <EditText android:id="@+id/password" android:hint="Password" android:inputType="textPassword" android:layout\_width="match\_parent" android:layout\_height="wrap\_content" /> <Button android:id="@+id/loginBtn" android:text="Login" android:layout\_width="match\_parent" android:layout\_height="wrap\_content" />

&#x20;\*/ 

// ========================= // =========================

