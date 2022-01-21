# Android_CheckBox
Using CheckBox in Android App

# Code

#### 1st Activity 
```
CheckBox ch1, ch2, ch3, ch4;

        ch1 = findViewById(R.id.checkBox1);
        ch2 = findViewById(R.id.checkBox2);
        ch3 = findViewById(R.id.checkBox3);
        ch4 = findViewById(R.id.checkBox4);

        //better way to handle multiple on click listener
        ch1.setOnClickListener(this);
        ch2.setOnClickListener(this);
        ch3.setOnClickListener(this);
        ch4.setOnClickListener(this);
        
        
        @Override
    public void onClick(View v) {
        switch (v.getId()) {
            case R.id.checkBox1:
                if (ch1.isChecked())
                    Toast.makeText(getApplicationContext(), "You selected Java", Toast.LENGTH_SHORT).show();
                break;

            case R.id.checkBox2:
                Toast.makeText(getApplicationContext(), "You Selected C/C++", Toast.LENGTH_SHORT).show();
                break;

            case R.id.checkBox3:
                Toast.makeText(getApplicationContext(), "You Selected Python", Toast.LENGTH_SHORT).show();
                break;

            case R.id.checkBox4:
                Toast.makeText(getApplicationContext(), "You Selected Dart", Toast.LENGTH_SHORT).show();
                break;
        }
    }
```

# App Highlight

<img src="app_images/checkBox Code.png" width="1000" /><br>

<img src="app_images/checkBox App1.png" width="300" /> <img src="app_images/checkBox App2.png" width="300" /><br>
