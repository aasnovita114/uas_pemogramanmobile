# uas_pemogramanmobile

<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Aas Novitasari</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210167</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A1</td>
  </tr>
  <tr>
    <td>Dosen</td>
    <td>Donny Maulana, S.Kom., M.M.S.I.</td>
  </tr>
</table>

 ## 1. Menu utama
 Pertama yang harus kita lakukan adalah mengganti tampilan menu utamanya dengan code yang baru agar ikon tombol berubah menjadi gambar, caranya adalah :

Jika awal pembuatan project kita memilih template Empty Views Activity, maka pada layout otomatis terbuat file activity_menu.xml dan pada java akan ada MenuActivity.java. Maka langsung saja kita buka activity_menu.xml, dan buat code seperti berikut ini:
 ```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">


    <RelativeLayout
        android:layout_width="500dp"
        android:layout_height="match_parent"
        android:background="@drawable/download__1_">

    </RelativeLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="100dp"
        android:layout_marginRight="16dp"
        android:orientation="vertical">

        <TextView
            android:id="@+id/textView"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:fontFamily="serif"
            android:text="Menu Program"
            android:textAlignment="center"
            android:textColor="@color/black"
            android:textSize="34sp"
            android:textStyle="bold" />

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu1"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView0"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/hello_world" />

                    <TextView
                        android:id="@+id/textView0"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Hello word"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu2"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView1"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/calculator" />

                    <TextView
                        android:id="@+id/textView1"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Count"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu3"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView2"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/movie" />

                    <TextView
                        android:id="@+id/textView2"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Scroll Movie"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu4"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/clock" />

                    <TextView
                        android:id="@+id/textView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Alarm"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:layout_margin="5dp"
            android:orientation="horizontal">

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu5"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView4"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/chat" />

                    <TextView
                        android:id="@+id/textView4"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Two Activity"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

            <androidx.cardview.widget.CardView
                android:id="@+id/cdMenu6"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/map" />

                    <TextView
                        android:id="@+id/textView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="Maps"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
            </androidx.cardview.widget.CardView>

        </LinearLayout>
    </LinearLayout>

</RelativeLayout>
```

* Setelah itu kita buka MenuActivity.java untuk menambahkan code intent untuk masing-masing tombol :
```
package com.aasapp;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        findViewById(R.id.cdMenu4).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                setAlarm();
            }
        });

        findViewById(R.id.cdMenu1).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolSatu ditekan, pindah ke HelloActivity
                Intent helloworld = new Intent(MainActivity.this, HelloActivity.class);
                startActivity(helloworld);
            }
        });

        findViewById(R.id.cdMenu2).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolDua ditekan, lakukan aksi yang diinginkan
                // Misalnya, pindah ke aktivitas lain atau jalankan fungsi khusus
                Intent toast = new Intent(MainActivity.this, CountActivity.class);
                startActivity(toast);
            }
        });

        findViewById(R.id.cdMenu3).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolDua ditekan, lakukan aksi yang diinginkan
                // Misalnya, pindah ke aktivitas lain atau jalankan fungsi khusus
                Intent sianida = new Intent(MainActivity.this, SianidaActivity.class);
                startActivity(sianida);
            }
        });

        findViewById(R.id.cdMenu5).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Ketika tombolDua ditekan, lakukan aksi yang diinginkan
                // Misalnya, pindah ke aktivitas lain atau jalankan fungsi khusus
                Intent twoactivity = new Intent(MainActivity.this, TwoActivity.class);
                startActivity(twoactivity);
            }
        });

        findViewById(R.id.cdMenu6).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Example location: Jakarta, Indonesia
                Uri geoLocation = Uri.parse("geo:-6.2088,106.8456");
                openMaps(geoLocation);
            }
        });
    }

    private void setAlarm() {
        Intent alarmIntent = new Intent(android.provider.AlarmClock.ACTION_SET_ALARM);
        // Add extra details for the alarm, e.g., alarm time, label, etc.
        // alarmIntent.putExtra(...
        startActivity(alarmIntent);
    }
    private void openMaps(Uri geoLocation) {
        Intent maps = new Intent(Intent.ACTION_VIEW);
        maps.setData(geoLocation);
        if (maps.resolveActivity(getPackageManager()) != null) {
            startActivity(maps);
        }
    }


}
```

## 2.AndroidManifest.xml
Didalam AndroidManifest.xml kita tambahkan semua java class dari semua project kita sebelumnya. Berikut nama java class dari berbagai project yang telah saya buat:

a. Project Hello World = HelloActivity.java

b. Project Count = CountActivity.java

c. Project Scroll Movie = SianidaActivity.java

d. Project TwoActivity = Reply.java dan Send.java

e. Project Set Alarm = MenuActivity.java

f. Project Maps = MenuActivity.java (karena merupakan Implicit Intent, jadi code untuk SetAlarm dan Maps langsung dibuat disini)

```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <uses-permission
        android:name="com.android.alarm.permission.SET_ALARM" />

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.Material3.Light"
        tools:targetApi="31">

        <activity
            android:name=".MenuActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.SET_ALARM" />
                <category android:name="android.intent.category.DEFAULT" />
                <action android:name="android.intent.action.VIEW" />
                <data android:scheme="geo" />
                <category android:name="android.intent.category.DEFAULT" />
            </intent-filter>
        </activity>

        <activity
            android:name=".SplashScreen"
            android:exported="true"
            android:theme="@style/Splash">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>

        <activity
            android:name=".HelloActivity"
            android:exported="true" />

        <activity
            android:name=".ReplyActivity"
            android:exported="true" />

        <activity
            android:name=".SendActivity"
            android:exported="true" />

        <activity
            android:name=".ToastActivity"
            android:exported="true" />

        <activity
            android:name=".SianidaActivity"
            android:exported="true" />
    </application>

</manifest>
```
## 3. Code All Project (XML files/res)
pada menu values:
* strings.xml

```
<resources>
    <string name="app_name">aasapp</string>
    <string name="Hello_World">Hello World!!</string>

    <string name="button_main">Send</string>
    <string name="editText_main">Enter Your Message Here</string>
    <string name="text_header">Message Received</string>
    <string name="buttton_second">Reply</string>
    <string name="editText_second">Enter Your Reply Here</string>
    <string name="text_header_reply">Reply Received</string>

    <string name="button_label_toast">Toast</string>
    <string name="button_label_count">Count</string>
    <string name="count_initial_value">1</string>
    <string name="toast_massage">Hello Toast!</string>
    <string name="button_label_restart">Restart</string>
    <string name="enter_fibonacci_limit">Masukkan Angka Limit</string>

    <string name="article_title"> Kasus Sianida</string>
    <string name="article_subtitle">ICE COLD!</string>

    <string name="article_text"> Film dokumenter Ice Cold: Murder, Coffee and Jessica Wongso memaparkan pertanyaan tak terjawab tentang persidangan yang dilalui Jessica Wongso. Dengan menyajikan perspektif baru, film ini hadir bertahun-tahun setelah kematian sahabat Jessica, Wayan Mirna Salihin.


Film ini menggambarkan bagaimana Jessica yang mengajak teman-temannya, termasuk Mirna, untuk bertemu setelah sekian lama tak berjumpa. Pertemuan di salah satu kafe di mal ibu kota tersebut pun berlangsung lancar, sebelum akhirnya Mirna pingsan sesaat setelah meminum kopi yang sebelumnya dipesan Jessica.Dokumenter ini turut menyajikan rekaman CCTV pada waktu kejadian, berbagai footage berita saat persidangan berlangsung, hingga wawancara eksklusif dengan beberapa sumber, termasuk Jessica Wongso.


Persidangan atas dugaan pembunuhan Mirna Salihin digelar lima bulan setelah kematiannya. Sidang tersebut melalui 32 kali persidangan dengan menghadirkan puluhan saksi di pengadilan. Hasilnya, Jessica Wongso divonis bersalah atas kematian Mirna dan dijatuhi hukuman 20 tahun penjara.
Kasus yang berjalan cukup lama tersebut menyita banyak perhatian dari masyarakat Indonesia. Musababnya, banyak misteri tak terjawab selama rangkaian persidangan yang panjang tersebut. Salah satunya adalah mengenai akses untuk mendapatkan bubuk sianida yang tidak bisa didapatkan oleh orang sembarangan. Selain itu, motif Jessica di balik pembunuhan tersebut pun belum menemukan jawabannya.


Film dokumenter buatan Netflix ini menyoroti rangkaian persidangan yang saat itu menjadi sidang pertama yang disiarkan secara langsung di berbagai stasiun televisi Indonesia. Selain itu, kasus ini juga diliput secara intens oleh media massa, baik nasional maupun internasional.Tak hanya itu, pihak rumah produksi Beach House Pictures juga berhasil mendapatkan akses untuk mewawancarai Jessica Wongso secara langsung dari balik tahanan. Dalam video trailer yang diluncurkannya, ditampilkan juga sejumlah wawancara eksklusif yang dilakukan dengan beberapa narasumber. Mulai dari ayah dan saudara kembar  Mirna Salihin, pengacara Jessica Wongso, jurnalis yang mendalami kasus tersebut, hingga bagaimana saat itu kasus ini begitu ramai diberitakan oleh media massa Indonesia dan internasional.</string>

</resources>
```
* color.xml

```
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="black">#FF000000</color>
    <color name="white">#FFFFFFFF</color>
    <color name="blue">#3700B3</color>
    <color name="pink">#FFC0CB</color>
    <color name="colorPrimary">#3F5185</color>
    <color name="colorPrimaryDark">#303F9F</color>
    <color name="colorAccent">#FF4081</color>
    <color name="birumuda">#ABCBFA</color>
    <color name ="purple">#E3A2ED</color>
    <color name="hijau">#92A676</color>
    <color name="biru">#8FC2EA</color>
    <color name="hijaumuda">#C2E69C</color>
    <color name="cream">#E6C18A</color>
    <color name="grey">#DACEC5</color>
</resources>
```
* Dimens.xml

```
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <dimen name="padding_regular">10dp</dimen>
    <dimen name="line_spacing">5sp</dimen>
</resources>
```
* themes.xml

```
<resources xmlns:tools="http://schemas.android.com/tools">
    <!-- Base application theme. -->
    <style name="SplashScreen" parent="Theme.MaterialComponents.DayNight.NoActionBar">
        <item name="android:windowBackground">@drawable/logo</item>
        <item name="android:statusBarColor">?attr/colorOnPrimary</item>
    </style>
</resources>
```
* Beckgroundlauncher.xml

```
<?xml version="1.0" encoding="utf-8"?>
<layer-list
    xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:drawable="@color/grey"/>
    <item>
        <bitmap
            android:src="@drawable/logo"
            android:gravity="center" />
    </item>
</layer-list>
```
## A. Code Project Hello World
* activity_hello.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".HelloActivity">

    <ImageView
        android:id="@+id/background"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:adjustViewBounds="true"
        android:background="@drawable/bg2"
        android:scaleType="centerCrop"
        tools:layout_editor_absoluteX="-16dp"
        tools:layout_editor_absoluteY="-152dp" />

    <TextView
        android:id="@+id/txthello"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:text="Hello World!!"
        android:textColor="@color/white"
        android:textSize="20pt"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.583"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.152"
        tools:ignore="TextSizeCheck" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
* HelloActivity.java
```
package com.aasapp;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

public class HelloActivity extends AppCompatActivity{
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_hello);
    }
}
```
## B. Code Project Count
* Activity_count.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:ignore="ExtraText"
    tools:context=".CountActivity">

    <ImageView
        android:id="@+id/background"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="@drawable/bg3"
        android:adjustViewBounds="true"
        android:scaleType="centerCrop" />


    <Button
        android:id="@+id/button_limit"
        android:layout_width="354dp"
        android:layout_height="76dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="16dp"
        android:layout_marginEnd="8dp"
        android:background="@color/cream"
        android:onClick="setLimit"
        android:text="Masukkan Angka Limit"
        android:textColor="@android:color/black"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.507"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_count"
        android:layout_width="173dp"
        android:layout_height="70dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="24dp"
        android:background="@color/cream"
        android:onClick="countUp"
        android:text="Count"
        android:textColor="@android:color/black"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.039"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_restart"
        android:layout_width="173dp"
        android:layout_height="72dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="24dp"
        android:background="@color/cream"
        android:onClick="back1"
        android:text="Restart"
        android:textColor="@android:color/black"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.965"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <TextView
        android:id="@+id/show_count"
        android:layout_width="305dp"
        android:layout_height="442dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:gravity="center_vertical"
        android:text="1"
        android:textAlignment="center"
        android:textColor="@color/white"
        android:textSize="160sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@id/button_count"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.505"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/button_limit"
        app:layout_constraintVertical_bias="0.51"
        tools:ignore="RtlCompat" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
* CountActivity.java
```
package com.aasapp;

import android.app.AlertDialog;
import android.content.DialogInterface;
import android.graphics.Color;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;


public class CountActivity extends AppCompatActivity {
    private TextView show_count;
    private int count = 1;
    private long fibNMinus1 = 1;
    private long fibNMinus2 = 1;
    private int limit = -1; // Inisialisasi limit dengan nilai default

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_count);

        show_count = findViewById(R.id.show_count);
    }

    public void countUp(View view) {
        if (count == 0) {
            show_count.setText("0");
        }
        else if (count == 1) {
            show_count.setText("1");
        }
        else {
            if (limit != -1 && count > limit) {
                // Jika count melebihi limit, atur ulang perhitungan
                count = 0;
                fibNMinus1 = 1;
                fibNMinus2 = 0;
                show_count.setText(getString(R.string.count_initial_value));
            }
            else {
                long fibCurrent = fibNMinus1 + fibNMinus2;
                fibNMinus2 = fibNMinus1;
                fibNMinus1 = fibCurrent;

                //Mengatur warna teks berdasarkan angka Fibonacci
                int colorResId = R.color.colorAccent; // Warna Default
                switch (count % 11) {
                    case 1:
                        colorResId = R.color.colorAccent; // Warna Pink Tua
                        break;
                    case 2:
                        colorResId = R.color.hijaumuda; // Warna Hijau Muda
                        break;
                    case 3:
                        colorResId = R.color.purple; // Warna Ungu
                        break;
                    case 4:
                        colorResId = R.color.blue; // Warna Salem
                        break;
                    case 5:
                        colorResId = R.color.birumuda; // Warna Biru Muda
                        break;
                    case 6 :
                        colorResId = R.color.cream; // Warna Kuning
                        break;
                    case 7:
                        colorResId = R.color.hijau; // Warna Hijau
                        break;
                    case 8:
                        colorResId = R.color.cream; // Warna Cream
                        break;
                    case 9:
                        colorResId = R.color.pink; // Warna Pink
                        break;
                    case 10:
                        colorResId = R.color.biru; // Warna Biru
                        break;
                    case 11:
                        colorResId = R.color.hijau; // Warna Orange
                        break;
                }
                show_count.setTextColor(getResources().getColor(colorResId));
                show_count.setText(String.valueOf(fibCurrent));
            }
        }

        count++;
    }

    public void back1(View view) {
        count = 1;
        fibNMinus1 = 1;
        fibNMinus2 = 0;
        show_count.setText(getString(R.string.count_initial_value));
    }

    public void setLimit(View view) {
        // Create and display a dialog to set the limit
        AlertDialog.Builder builder = new AlertDialog.Builder(this);
        builder.setTitle("Set Limit");

        final EditText input = new EditText(this);
        input.setInputType(android.text.InputType.TYPE_CLASS_NUMBER);
        builder.setView(input);

        builder.setPositiveButton("OK", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                // Get the limit from the input and set it for calculations
                String limitStr = input.getText().toString();
                limit = Integer.parseInt(limitStr);
            }
        });

        builder.setNegativeButton("Cancel", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                dialog.cancel();
            }
        });

        builder.show();
    }
}
```
## c. Code Project Sianida
* Activity_scrollmovie.xml
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:tools="http://schemas.android.com/tools"
    tools:context=".SianidaActivity">

    <TextView
        android:id="@+id/article_heading"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="@color/grey"
        android:padding="@dimen/padding_regular"
        android:text="@string/article_title"
        android:textAppearance="@android:style/TextAppearance.DeviceDefault.Large"
        android:textColor="@android:color/white"
        android:textStyle="bold" />

    <ScrollView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/article_heading">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:orientation="vertical">

            <TextView
                android:id="@+id/article_subheading"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:padding="@dimen/padding_regular"
                android:text="@string/article_subtitle"
                android:textAlignment="center"
                android:textAppearance="@android:style/TextAppearance.DeviceDefault"
                android:textColor="#FF000000" />

            <TextView
                android:id="@+id/article"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:autoLink="web"
                android:lineSpacingExtra="@dimen/line_spacing"
                android:padding="@dimen/padding_regular"
                android:text="@string/article_text"
                tools:ignore="VisualLintLongText" />
        </LinearLayout>
    </ScrollView>
</RelativeLayout>
```
* SianidaActivity.java
```
package com.aasapp;

import android.os.Bundle;

import androidx.appcompat.app.AppCompatActivity;

public class SianidaActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_scrollmovie);
    }
}
```
## D. Code Project Two Activity
* Activity_Twoactivity.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    tools:context=".TwoActivity">

    <ImageView
        android:id="@+id/background"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:adjustViewBounds="true"
        android:scaleType="centerCrop"
        android:src="@drawable/bg4" />

    <TextView
        android:id="@+id/text_header_reply"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="16dp"
        android:text="@string/text_header_reply"
        android:textAppearance="@style/TextAppearance.AppCompat.Medium"
        android:textStyle="bold"
        android:visibility="invisible"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>

    <TextView
        android:id="@+id/text_message_reply"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="8dp"
        android:visibility="invisible"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/text_header_reply" />

    <Button
        android:id="@+id/button_main"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="16dp"
        android:layout_marginRight="16dp"
        android:text="@string/button_main"
        android:background="@color/grey"
        android:onClick="LaunchSecondActivity"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        tools:ignore="UsingOnClickInXml"/>

    <EditText
        android:id="@+id/editText_main"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="16dp"
        android:ems="10"
        android:hint="@string/editText_main"
        android:inputType="textLongMessage"
        android:minHeight="48dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button_main"
        app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
* Twoactivity.java
```
package com.aasapp;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.util.Log;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class TwoActivity extends AppCompatActivity {

    private static final String LOG_TAG = TwoActivity.class.getSimpleName();

    public static final String EXTRA_MESSAGE = "com.example.android.Two2Activity.extra.MESSAGE";

    public static final int TEXT_REQUEST = 1;

    private EditText mMessageEditText;

    private TextView mReplyHeadTextView;

    private TextView mReplyTextView;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_twoactivity);

        mMessageEditText = findViewById(R.id.editText_main);
        mReplyHeadTextView = findViewById(R.id.text_header_reply);
        mReplyTextView = findViewById(R.id.text_message_reply);
    }

    public void LaunchSecondActivity(View view) {
        Log.d(LOG_TAG, "Button clicked!");
        Intent intent = new Intent(this, Two2Activity.class);
        String message = mMessageEditText.getText().toString();
        intent.putExtra(EXTRA_MESSAGE, message);
        startActivityForResult(intent, TEXT_REQUEST);
    }

    @Override
    public void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);

        if (requestCode == TEXT_REQUEST) {
            if (resultCode == RESULT_OK) {
                String reply = data.getStringExtra(Two2Activity.EXTRA_REPLY);

                mReplyHeadTextView.setVisibility(View.VISIBLE);
                mReplyTextView.setText(reply);
                mReplyTextView.setVisibility(View.VISIBLE);
            }
        }
    }
}
```
* Activity_two2activity.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    tools:context=".Two2Activity">

    <ImageView
        android:id="@+id/background"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:adjustViewBounds="true"
        android:scaleType="centerCrop"
        android:src="@drawable/bg4" />

    <TextView
        android:id="@+id/text_header"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="16dp"
        android:text="@string/text_header"
        android:textAppearance="@style/TextAppearance.AppCompat.Medium"
        android:textStyle="bold"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/text_message"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="8dp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/text_header" />

    <Button
        android:id="@+id/button_second"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="16dp"
        android:layout_marginRight="16dp"
        android:text="@string/buttton_second"
        android:onClick="returnReply"
        android:background="@color/grey"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <EditText
        android:id="@+id/editText_second"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="16dp"
        android:ems="10"
        android:hint="@string/editText_second"
        android:inputType="textLongMessage"
        android:minHeight="48dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button_second"
        app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
* Two2activity.java
```
package com.aasapp;

import android.content.Intent;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

import androidx.appcompat.app.AppCompatActivity;

public class Two2Activity extends AppCompatActivity {

    public static final String EXTRA_REPLY ="com.example.android.Two2Activity.extra.REPLY";
    public static final String EXTRA_MESSAGE ="com.example.android.Two2Activity.extra.MESSAGE";
    private EditText mReply;

    @Override
    protected void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_two2activity);

        mReply = findViewById(R.id.editText_second);

        Intent intent = getIntent();
        String message = intent.getStringExtra(Two2Activity.EXTRA_MESSAGE);

        TextView textView = findViewById(R.id.text_message);
        textView.setText(message);
    }
    public void returnReply(View view){
        String reply = mReply.getText().toString();
        Intent replyIntent = new Intent();
        setResult(RESULT_OK, replyIntent);
        finish();
    }
}
```

## E.Code Project SetAlarm dan Maps
* Set Alarm
```
<androidx.cardview.widget.CardView
                android:id="@+id/cdMenu4"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/alarm" />

                    <TextView
                        android:id="@+id/textView3"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:onClick="setAlarm"
                        android:text="SET ALARM"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
```
* Maps
```
<androidx.cardview.widget.CardView
                android:id="@+id/cdMenu6"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_margin="10dp"
                android:layout_weight="1"
                app:cardCornerRadius="20dp"
                app:cardElevation="7dp">

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical">

                    <ImageView
                        android:id="@+id/imageView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_margin="16dp"
                        android:layout_weight="1"
                        app:srcCompat="@drawable/maps" />

                    <TextView
                        android:id="@+id/textView5"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:fontFamily="serif"
                        android:text="MAPS"
                        android:textAlignment="center"
                        android:textSize="18dp"
                        android:textStyle="bold" />
                </LinearLayout>
```
Lalu tambahkan code Implicit Intent pada MenuActivity.java :
* SetAlarm
```
findViewById(R.id.cdMenu4).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                setAlarm();
            }
        });
private void setAlarm() {
        Intent alarmIntent = new Intent(android.provider.AlarmClock.ACTION_SET_ALARM);
        // Add extra details for the alarm, e.g., alarm time, label, etc.
        // alarmIntent.putExtra(...
        startActivity(alarmIntent);
    }
```
* Maps
```
findViewById(R.id.cdMenu6).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // Example location: Jakarta, Indonesia
                Uri geoLocation = Uri.parse("geo:-6.2088,106.8456");
                openMaps(geoLocation);
            }
        });
private void openMaps(Uri geoLocation) {
        Intent maps = new Intent(Intent.ACTION_VIEW);
        maps.setData(geoLocation);
        if (maps.resolveActivity(getPackageManager()) != null) {
            startActivity(maps);
        }
    }
```
Selanjutnya buka AndroidManifest.xml dan tambahkan code untuk izin membuka Alarm :
```
<uses-permission android:name="com.android.alarm.permission.SET_ALARM" />
```
Tambahkan code berikut pada bagian application agar set alarm dapat berjalan :
```
<activity
            android:name=".MenuActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.SET_ALARM" />
                <category android:name="android.intent.category.DEFAULT" />
                <action android:name="android.intent.action.VIEW" />
                <data android:scheme="geo" />
                <category android:name="android.intent.category.DEFAULT" />
            </intent-filter>
        </activity>
```


