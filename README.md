# Dicee-Android
<img src="https://github.com/PratyayMallik1006/Dicee-Android/blob/main/Dicee.jpeg?raw=true" height="600" style="float: left">

## Notes:
1. In activity_main.xml
```xml
<ImageView  
  android:id="@+id/image_leftDice"  
  android:layout_width="wrap_content"  
  android:layout_height="wrap_content"  
  android:layout_weight="1"  
  app:srcCompat="@drawable/dice2" />
```
2. MainActivity.java
```java
 @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button rollButton;
        rollButton = (Button) findViewById(R.id.rollButton);

        ImageView leftDice = (ImageView) findViewById(R.id.image_leftDice);
        
        final int[] diceArray ={  
          R.drawable.dice1, 
          R.drawable.dice2,
          R.drawable.dice3
      };
//int array of resId

leftDice.setImageResource(diceArray[number]); // int resId

```
