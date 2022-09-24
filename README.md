# Android_CheckBox
Using CheckBox in Android App

This topic is a part of [My Complete Andorid Course](https://github.com/ananddasani/Android_Apps)

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

![checkBox App1](https://user-images.githubusercontent.com/74413402/192092749-461ab8b6-997c-4e92-adb5-57190cd2b43d.png)
![checkBox App2](https://user-images.githubusercontent.com/74413402/192092750-fe95906f-562f-4e58-97a9-706be800ed5d.png)
![checkBox Code](https://user-images.githubusercontent.com/74413402/192092752-9ca22103-9534-4248-a73c-d019a5d004c6.png)
