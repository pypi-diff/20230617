# Comparing `tmp/sb6-0.0.3.tar.gz` & `tmp/sb6-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb6-0.0.3.tar", last modified: Thu Jun 15 14:25:38 2023, max compression
+gzip compressed data, was "sb6-0.0.4.tar", last modified: Sat Jun 17 13:04:26 2023, max compression
```

## Comparing `sb6-0.0.3.tar` & `sb6-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:25:38.998940 sb6-0.0.3/
--rw-rw-rw-   0        0        0     1067 2023-04-11 12:54:43.000000 sb6-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      462 2023-06-15 14:25:38.998940 sb6-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-05-12 01:06:50.000000 sb6-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 14:25:38.998940 sb6-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-06-15 14:24:22.000000 sb6-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:25:38.983314 sb6-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 14:25:38.998940 sb6-0.0.3/src/sb6.egg-info/
--rw-rw-rw-   0        0        0      462 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-15 14:25:38.000000 sb6-0.0.3/src/sb6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   138791 2023-06-15 14:20:16.000000 sb6-0.0.3/src/sb6.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:04:26.340268 sb6-0.0.4/
+-rw-rw-rw-   0        0        0     1067 2023-04-11 12:54:43.000000 sb6-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      462 2023-06-17 13:04:26.339260 sb6-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-05-12 01:06:50.000000 sb6-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 13:04:26.340268 sb6-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-06-17 13:04:13.000000 sb6-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:04:26.320739 sb6-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-17 13:04:26.339260 sb6-0.0.4/src/sb6.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-06-17 13:04:26.000000 sb6-0.0.4/src/sb6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-06-17 13:04:26.000000 sb6-0.0.4/src/sb6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:04:26.000000 sb6-0.0.4/src/sb6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-17 13:04:26.000000 sb6-0.0.4/src/sb6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-17 13:04:26.000000 sb6-0.0.4/src/sb6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   141676 2023-06-17 13:02:59.000000 sb6-0.0.4/src/sb6.py
```

### Comparing `sb6-0.0.3/LICENSE` & `sb6-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sb6-0.0.3/setup.py` & `sb6-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sb6",
-    version="0.0.3",
+    version="0.0.4",
     description='chatbot',
     license='MIT',
     author="aiml department",
     author_email="aiml@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `sb6-0.0.3/src/sb6.py` & `sb6-0.0.4/src/sb6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1322,14 +1322,50 @@
 import sklearn.metrics as sm
 print("The accuracy score of EM:", sm.accuracy_score(y['Targets'], y_cluster_gmm))
 
 plt.subplot(1, 3, 3)        # Plot the clusters predicted by GMM
 plt.scatter(x['petal_length'], x['petal_width'], c=colormap[y_cluster_gmm], s=40)
 plt.title('GMM Clusters')
 plt.show()
+
+
+'''
+from sklearn.mixture import GaussianMixture
+from sklearn.datasets import load_iris
+import sklearn.metrics as sm
+import pandas as pd
+import numpy as np
+import matplotlib.pyplot as plt
+from sklearn import preprocessing
+
+dataset = load_iris()
+X = pd.DataFrame(dataset.data)
+X.columns = ['Sepal_Length','Sepal_Width','Petal_Length','Petal_Width']
+y = pd.DataFrame(dataset.target)
+y.columns=['Targets']
+
+plt.figure(figsize=(14,7))
+colormap = np.array(['red','lime','black'])
+
+plt.subplot(1,3,1)
+plt.scatter(X.Petal_Length,X.Petal_Width,c=colormap[y.Targets],s=40)
+plt.title("Real")
+
+scaler=preprocessing.StandardScaler()
+scaler.fit(X)
+xsa = scaler.transform(X)
+xs=pd.DataFrame(xsa,columns=X.columns)
+gmm=GaussianMixture(n_components=3)
+gmm.fit(xs)
+y_cluster_gmm=gmm.predict(xs)
+print('The accuracy score of EM: ',sm.accuracy_score(y,y_cluster_gmm))
+plt.subplot(1,3,3)
+plt.scatter(X.Petal_Length,X.Petal_Width,c=colormap[y_cluster_gmm],s=40)
+plt.title("GMM Classification")
+'''
         """)
 
 class mlfull():
     """
 pg1() : FIND-S : Finding a Maximally Specific (0) Hypothesis  
     Implement and demonstrate the FIND-S algorithm for finding the most specific hypothesis based on a given set of training data samples. 
     Read the training data from a .CSV file and show the output for test cases. 
@@ -3053,15 +3089,16 @@
         """)
         
     def wallpaper():
         """
     Develop an application to set an image as wallpaper. On click of a button, the wallpaper image should start to change randomly every 30 seconds.
         """
         print(r"""
-package com.example.wallpaper;
+  //MainActivity.java
+package com.example.project7;
 import androidx.appcompat.app.AppCompatActivity;
 import android.app.WallpaperManager;
 import android.graphics.Bitmap;
 import android.graphics.drawable.BitmapDrawable;
 import android.graphics.drawable.Drawable;
 import android.os.Bundle;
 import android.view.View;
@@ -3079,57 +3116,107 @@
     protected void onCreate(Bundle savedInstanceState) {
         super.onCreate(savedInstanceState);
         setContentView(R.layout.activity_main);
         b1 = findViewById(R.id.click);
         Mytimer = new Timer();
         Mywall = WallpaperManager.getInstance(this);
         b1.setOnClickListener(new View.OnClickListener() {
-        @Override
-        public void onClick(View view) {
-            changewallpaper();
-        }
+            @Override
+            public void onClick(View view) {
+                changewallpaper();
+            }
         });
     }
     private void changewallpaper() {
         Mytimer.schedule(new TimerTask() {
-        @Override
-        public void run() {
-            if (nextpaper == 1) {
-            Mydraw = getResources().getDrawable(R.drawable.a);
-            nextpaper = 2;
-            } else if (nextpaper == 2) {
-            Mydraw = getResources().getDrawable(R.drawable.c);
-            nextpaper = 3;
-            } else if (nextpaper == 3) {
-            Mydraw = getResources().getDrawable(R.drawable.d);
-            nextpaper = 4;
-            } else if (nextpaper == 4) {
-            Mydraw = getResources().getDrawable(R.drawable.e);
-            nextpaper = 5;
-            } else if (nextpaper == 5)
-            System.exit(0);
-            Bitmap wallpaper = ((BitmapDrawable) Mydraw).getBitmap();
-            try {
-            Mywall.setBitmap(wallpaper);
-            } catch (IOException e) {
-            e.printStackTrace();
+            @Override
+            public void run() {
+                if (nextpaper == 1) {
+                    Mydraw = getResources().getDrawable(R.drawable.a);
+                    nextpaper = 2;
+                } else if (nextpaper == 2) {
+                    Mydraw = getResources().getDrawable(R.drawable.b);
+                    nextpaper = 3;
+                } else if (nextpaper == 3) {
+                    Mydraw = getResources().getDrawable(R.drawable.c);
+                    nextpaper = 4;
+                } else if (nextpaper == 4) {
+                    Mydraw = getResources().getDrawable(R.drawable.d);
+                    nextpaper = 5;
+                } else if (nextpaper == 5)
+                    System.exit(0);
+                Bitmap wallpaper = ((BitmapDrawable) Mydraw).getBitmap();
+                try {
+                    Mywall.setBitmap(wallpaper);
+                } catch (IOException e) {
+                    e.printStackTrace();
+                }
             }
-        }
-        }, 0, 1000);
+        }, 0, 3000);
     }
 }
+
+
+    // activity_main.xml
+<?xml version="1.0" encoding="utf-8"?>
+<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    tools:context=".MainActivity">
+
+    <TextView
+        android:id="@+id/textView"
+        android:layout_width="409dp"
+        android:layout_height="wrap_content"
+        android:gravity="center"
+        android:text="CHANGING WALLPAPER APPLICATION"
+        android:textColor="@color/black"
+        android:textSize="34sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.292" />
+
+    <Button
+        android:id="@+id/click"
+        android:layout_width="346dp"
+        android:layout_height="84dp"
+        android:text="CLICK HERE TO CHANGE WALLPAPER"
+        android:textSize="20sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.492"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/textView"
+        app:layout_constraintVertical_bias="0.254" />
+
+</androidx.constraintlayout.widget.ConstraintLayout>
         """)
         
-    def parse_xml_json_files():
+    def parse_xml_json():
         """
         parse xml json files
+        
+        advice
+        - create assets  folder in app 
+        - create city.json file in assets folder
+        - create city.xml file in assets folder
         """
         print(r"""
+ advice
+- create assets  folder in app 
+- create city.json file in assets folder
+- create city.xml file in assets folder
+
+
     //MainActivity.java
-package com.example.parse;
+package com.example.project8;
 import androidx.appcompat.app.AppCompatActivity;
 import android.os.Bundle;
 import android.view.View;
 import android.widget.TextView;
 import android.widget.Toast;
 import org.json.JSONArray;
 import org.json.JSONObject;
@@ -3157,184 +3244,176 @@
             DocumentBuilder documentBuil=documentfact.newDocumentBuilder();
             Document docu=documentBuil.parse(is);
             StringBuilder stringbuild=new StringBuilder();
             stringbuild.append("XML DATA");
             stringbuild.append("\n...........\n");
             NodeList nodeList=docu.getElementsByTagName("place");
             for(int i=0;i<nodeList.getLength();i++){
-            Node node=nodeList.item(i);
-            if(node.getNodeType()==Node.ELEMENT_NODE){
-            Element element=(Element) node;
-            stringbuild.append("\n city name:").append(getvalue("city",element));
-            stringbuild.append("\n latitude:").append(getvalue("lat",element));
-            stringbuild.append("\n longitude:").append(getvalue("long",element));
-            stringbuild.append("\n temperature:").append(getvalue("temp",element));
-            stringbuild.append("\n humidity:").append(getvalue("hum",element));
-            stringbuild.append("\n .........\n");
-            }
+                Node node=nodeList.item(i);
+                if(node.getNodeType()==Node.ELEMENT_NODE){
+                    Element element=(Element) node;
+                    stringbuild.append("\n city name :").append(getvalue("city",element));
+                    stringbuild.append("\n latitude :").append(getvalue("lat",element));
+                    stringbuild.append("\n longitude :").append(getvalue("long",element));
+                    stringbuild.append("\n temperature :").append(getvalue("temp",element));
+                    stringbuild.append("\n humidity :").append(getvalue("hum",element));
+                    stringbuild.append("\n .........\n");
+                }
             }
             tv1.setText(stringbuild.toString());
         }catch (Exception e){
             e.printStackTrace();
             Toast.makeText(this, "Error", Toast.LENGTH_SHORT).show();
         }
     }
     public void parsejson(View view){
-    String json;
-    StringBuilder stringbuild=new StringBuilder();
-    try{
-        InputStream is =getAssets().open("city.json");
-        int size=is.available();
-        byte[] buffer=new byte[size];
-        is.read(buffer);
-        json=new String(buffer, StandardCharsets.UTF_8);
-        JSONArray jsonarry=new JSONArray(json);
-        stringbuild.append("JSON DATA");
-        stringbuild.append("\n..........\n");
-        for(int i=0;i<jsonarry.length();i++){
-            JSONObject jsonObject=jsonarry.getJSONObject(i);
-            stringbuild.append("\n name : " ).append(jsonObject.getString("city"));
-            stringbuild.append("\n latitude : ").append(jsonObject.getString("lat"));
-            stringbuild.append("\n longitude : ").append(jsonObject.getString("long"));
-            stringbuild.append("\n temperature : ").append(jsonObject.getString("temp"));
-            stringbuild.append("\n humidity : ").append(jsonObject.getString("hum"));
+        String json;
+        StringBuilder stringbuild=new StringBuilder();
+        try{
+            InputStream is =getAssets().open("city.json");
+            int size=is.available();
+            byte[] buffer=new byte[size];
+            is.read(buffer);
+            json=new String(buffer, StandardCharsets.UTF_8);
+            JSONArray jsonarry=new JSONArray(json);
+            stringbuild.append("JSON DATA");
             stringbuild.append("\n..........\n");
+            for(int i=0;i<jsonarry.length();i++){
+                JSONObject jsonObject=jsonarry.getJSONObject(i);
+                stringbuild.append("\n city name : " ).append(jsonObject.getString("city"));
+                stringbuild.append("\n latitude : ").append(jsonObject.getString("lat"));
+                stringbuild.append("\n longitude : ").append(jsonObject.getString("long"));
+                stringbuild.append("\n temperature : ").append(jsonObject.getString("temp"));
+                stringbuild.append("\n humidity : ").append(jsonObject.getString("hum"));
+                stringbuild.append("\n..........\n");
+            }
+            tv2.setText(stringbuild.toString());
+        }catch (Exception e){
+            e.printStackTrace();
+            Toast.makeText(this, "error", Toast.LENGTH_SHORT).show();
         }
-        tv2.setText(stringbuild.toString());
-    }catch (Exception e){
-        e.printStackTrace();
-        Toast.makeText(this, "error", Toast.LENGTH_SHORT).show();
     }
-    }
-    private String getvalue(String tag,Element element)
-    {
+    private String getvalue(String tag,Element element){
         return element.getElementsByTagName(tag).item(0).getChildNodes().item(0).getNodeValue();
     }
 }
 
- // activity_main.xml
- 
-package com.example.parse;
-import androidx.appcompat.app.AppCompatActivity;
-import android.os.Bundle;
-import android.view.View;
-import android.widget.TextView;
-import android.widget.Toast;
-import org.json.JSONArray;
-import org.json.JSONObject;
-import org.w3c.dom.Document;
-import org.w3c.dom.Element;
-import org.w3c.dom.Node;
-import org.w3c.dom.NodeList;
-import java.io.InputStream;
-import java.nio.charset.StandardCharsets;
-import javax.xml.parsers.DocumentBuilder;
-import javax.xml.parsers.DocumentBuilderFactory;
-public class MainActivity extends AppCompatActivity {
-    TextView tv1,tv2;
-    @Override
-    protected void onCreate(Bundle savedInstanceState) {
-        super.onCreate(savedInstanceState);
-        setContentView(R.layout.activity_main);
-        tv1=findViewById(R.id.tv1);
-        tv2=findViewById(R.id.tv2);
-    }
-    public void parsexml(View view){
-    try{
-InputStream is=getAssets().open("city.xml");
-DocumentBuilderFactory documentfact=DocumentBuilderFactory.newInstance();
-DocumentBuilder documentBuil=documentfact.newDocumentBuilder();
-Document docu=documentBuil.parse(is);
-StringBuilder stringbuild=new StringBuilder();
-stringbuild.append("XML DATA");
-stringbuild.append("\n...........\n");
-NodeList nodeList=docu.getElementsByTagName("place");
-for(int i=0;i<nodeList.getLength();i++){
-    Node node=nodeList.item(i);
-    if(node.getNodeType()==Node.ELEMENT_NODE){
-        Element element=(Element) node;
-        stringbuild.append("\n city name:").append(getvalue("city",element));
-        stringbuild.append("\n latitude:").append(getvalue("lat",element));
-        stringbuild.append("\n longitude:").append(getvalue("long",element));
-        stringbuild.append("\n temperature:").append(getvalue("temp",element));
-        stringbuild.append("\n humidity:").append(getvalue("hum",element));
-        stringbuild.append("\n .........\n");
-    }
-}
-tv1.setText(stringbuild.toString());
-}catch (Exception e){
-    e.printStackTrace();
-    Toast.makeText(this, "Error", Toast.LENGTH_SHORT).show();
-}
-}
-public void parsejson(View view){
-    String json;
-    StringBuilder stringbuild=new StringBuilder();
-    try{
-        InputStream is =getAssets().open("city.json");
-        int size=is.available();
-        byte[] buffer=new byte[size];
-        is.read(buffer);
-        json=new String(buffer, StandardCharsets.UTF_8);
-        JSONArray jsonarry=new JSONArray(json);
-        stringbuild.append("JSON DATA");
-        stringbuild.append("\n..........\n");
-        for(int i=0;i<jsonarry.length();i++){
-            JSONObject jsonObject=jsonarry.getJSONObject(i);
-            stringbuild.append("\n name : " ).append(jsonObject.getString("city"));
-            stringbuild.append("\n latitude : ").append(jsonObject.getString("lat"));
-            stringbuild.append("\n longitude : ").append(jsonObject.getString("long"));
-            stringbuild.append("\n temperature : ").append(jsonObject.getString("temp"));
-            stringbuild.append("\n humidity : ").append(jsonObject.getString("hum"));
-            stringbuild.append("\n..........\n");
-        }
-        tv2.setText(stringbuild.toString());
-    }catch (Exception e){
-    e.printStackTrace();
-    Toast.makeText(this, "error", Toast.LENGTH_SHORT).show();
-    }
-    }
-    private String getvalue(String tag,Element element)
-    {
-        return element.getElementsByTagName(tag).item(0).getChildNodes().item(0).getNodeValue();
-    }
-}
 
-//txt.xml
+//assets/city.xml
 <record>
-<place>
-<city>Mysore</city>
-<lat>75.55</lat>
-<long>76.639</long>
-<temp>22</temp>
-<hum>90</hum>
-</place><place>
-<city>Puttur</city>
-<lat>12.2</lat>
-<long>16.539</long>
-<temp>25</temp>
-<hum>70</hum>
-</place>
+    <place>
+        <city>Mysore</city>
+        <lat>75.55</lat>
+        <long>76.639</long>
+        <temp>22</temp>
+        <hum>90</hum>
+    </place>
+    <place>
+        <city>puttur</city>
+        <lat>12.2</lat>
+        <long>16.539</long>
+        <temp>25</temp>
+        <hum>70</hum>
+    </place>
 </record>
 
-// txt2.json
-[{ "
-city":"mysore",
-"lat":"75.55",
-"long":"76.639",
-"temp":"22",
-"hum":"90"
-},
-{ "
-city":"puttur",
-"lat":"12.2",
-"long":"16.539",
-"temp":"25",
-"hum":"70"
-}]
+
+//assets/city.json
+
+[
+  {
+    "city": "mysore",
+    "lat": "75.55",
+    "long": "76.639",
+    "temp": "22",
+    "hum": "90"
+  },
+  {
+    "city": "puttur",
+    "lat": "12.2",
+    "long": "16.539",
+    "temp": "25",
+    "hum": "70"
+  }
+]
+
+
+ // activity_main.xml
+ <?xml version="1.0" encoding="utf-8"?>
+<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    tools:context=".MainActivity">
+
+    <TextView
+        android:id="@+id/tv2"
+        android:layout_width="185dp"
+        android:layout_height="444dp"
+        android:gravity="center"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.964"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.867" />
+
+    <Button
+        android:id="@+id/bt2"
+        android:layout_width="177dp"
+        android:layout_height="52dp"
+        android:onClick="parsejson"
+        android:text="PARSING JSON DATA"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.931"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.262" />
+
+    <TextView
+        android:layout_width="360dp"
+        android:layout_height="75dp"
+        android:gravity="center"
+        android:text="PARSING XML AND JSON DATA"
+        android:textSize="24sp"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.49"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.077" />
+
+    <Button
+        android:id="@+id/bt1"
+        android:layout_width="177dp"
+        android:layout_height="52dp"
+        android:onClick="parsexml"
+        android:text="PARSING XML DATA"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.05"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.262" />
+
+    <TextView
+        android:id="@+id/tv1"
+        android:layout_width="185dp"
+        android:layout_height="444dp"
+        android:gravity="center"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.017"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        app:layout_constraintVertical_bias="0.867" />
+
+</androidx.constraintlayout.widget.ConstraintLayout>
         """)
     
     def texttospeech():
         """
     Develop a simple application “convert text to speech” that converts the user input text into voice.
         """
         print(r"""
```

