# helloworld
This is the first Android Project

1.创建第一个Android工程 

2.为了更直观地认识Activity生命周期，在MainActivity中重写Activity的生命周期方法，并在每一个方法中打印出Log以便观察。

3.关键代码如下：

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.i("MainActivityLife","调用onCreate（）");
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.i("MainActivityLife","调用onStart（）");
    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.i("MainActivityLife","调用onResume（）");
    }
    @Override
    protected void onPause(){
        super.onPause();
        Log.i("MainActivityLife","调用onPause（）");
    }
    @Override
    protected void onDestroy(){
        super.onDestroy();
        Log.i("MainActivityLife","调用onDestroy（）");
    }
    @Override
    protected void onRestart(){
        super.onRestart();
        Log.i("MainActivityLife","调用onRestart（）");
    }
}



以下为实验截图：

![Image text](https://github.com/chenzifeng123/image/blob/master/001.png)

![Image text](https://github.com/chenzifeng123/image/blob/master/002.jpg)

