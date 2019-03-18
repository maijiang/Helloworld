# Helloworld

1.运行Helloworld,验证Activity的生命周期
--
MainActivity.java
--
    package com.example.lenovo.helloworld;

    import android.support.v7.app.AppCompatActivity;
    import android.os.Bundle;
    import android.util.Log;

    public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.i("MainActivity","调用onCreate()");
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.i("MainActivity","调用onStart()");

    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.i("MainActivity","调用onResume()");

    }
    @Override
    protected  void onPause(){
        super.onPause();
        Log.i("MainActivity","调用onPause()");
    }
    @Override
    protected  void onStop(){
        super.onStop();
        Log.i("MainActivity","调用onStop()");
    }
    @Override
    protected void onDestroy(){
        super.onDestroy();
        Log.i("MainActivity","调用onDestroy()");
    }
    @Override
    protected void onRestart(){
        super.onRestart();
        Log.i("MainActivity","调用onRestart()");
    }
    }
运行结果：
--
1.Helloworld
![Image text](https://github.com/maijiang/Helloworld/blob/master/hello.PNG)
    <br>
2.生命周期
![Image text](https://github.com/maijiang/Helloworld/blob/master/act_life.PNG)
