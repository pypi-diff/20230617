# Comparing `tmp/skmetpy-0.0.5.tar.gz` & `tmp/skmetpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.0.5.tar", last modified: Sat Jun 17 16:12:29 2023, max compression
+gzip compressed data, was "skmetpy-0.0.6.tar", last modified: Sat Jun 17 16:17:32 2023, max compression
```

## Comparing `skmetpy-0.0.5.tar` & `skmetpy-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:12:29.227377 skmetpy-0.0.5/
--rw-rw-rw-   0        0        0      259 2023-06-17 16:12:29.226705 skmetpy-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:12:29.220699 skmetpy-0.0.5/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.5/nunpy/__init__.py
--rw-rw-rw-   0        0        0    19070 2023-06-17 16:12:21.000000 skmetpy-0.0.5/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-17 16:12:29.227377 skmetpy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-17 16:12:27.000000 skmetpy-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:12:29.224704 skmetpy-0.0.5/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 16:17:32.665884 skmetpy-0.0.6/
+-rw-rw-rw-   0        0        0      259 2023-06-17 16:17:32.665884 skmetpy-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 16:17:32.659893 skmetpy-0.0.6/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.6/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    17657 2023-06-17 16:17:23.000000 skmetpy-0.0.6/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:17:32.665884 skmetpy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-17 16:17:30.000000 skmetpy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:17:32.664883 skmetpy-0.0.6/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.0.5/nunpy/rechape.py` & `skmetpy-0.0.6/nunpy/rechape.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 def list():
     print(f"1 - list() \n"
-          f"2 - list_1()\n"
-          f"3 - list_2()\n"
-          f"4 - pasos_1()\n"
-          f"5 - pasos_2()\n"
+          f"2 - list1()\n"
+          f"3 - list2()\n"
+          f"4 - pasos1()\n"
+          f"5 - pasos2()\n"
           f"6 - carga1()\n"
           f"7 - hold1()\n"
           f"8 - norm1()\n"
           f"9 - ini1()\n"
           f"10 - fordw1()\n"
           f"11 - cost1()\n"
           f"12 - grad1()\n"
@@ -22,30 +22,30 @@
           f"21 - recom2()\n"
           f"22 - simi2()\n"
           f"23 - km2()\n"
           f"24 - checkG2()\n")
 
 
 def list1():
-    print(f"1 - pasos_1()\n"
+    print(f"1 - pasos1()\n"
           f"2 - carga1()\n"
           f"3 - hold1()\n"
           f"4 - norm1()\n"
           f"5 - ini1()\n"
           f"6 - fordw1()\n"
           f"7 - cost1()\n"
           f"8 - grad1()\n"
           f"9 - fmin1()\n"
           f"10 - unroll1()\n"
           f"11 - pred1()\n"
           )
 
 
 def list2():
-    print(f"1 - pasos_2()\n"
+    print(f"1 - pasos2()\n"
           f"2 - carga2()\n"
           f"3 - rank2()\n"
           f"4 - cost2()\n"
           f"5 - grad2()\n"
           f"6 - fmin2()\n"
           f"7 - recom2()\n"
           f"8 - simi2()\n"
@@ -94,31 +94,26 @@
 
     print(string)
 
 
 def hold1():
     string = '''
             def holdout(X, y, percentage=0.75):
-                # Obtenemos los datos del X_training con la función sample
                 X_training = X.sample(round(percentage * len(X)))
 
-                # Utilizamos los mismos indices de X_training para y_training
                 y_training = y.iloc[X_training.index]
 
-                # Utilizamos los índices que no estén en X_training para los tests
                 X_test = X.iloc[~X.index.isin(X_training.index)]
                 y_test = y.iloc[~y.index.isin(y_training.index)]
 
-                # Reseteamos los índices
                 X_training = X_training.reset_index(drop=True)
                 y_training = y_training.reset_index(drop=True)
                 X_test = X_test.reset_index(drop=True)
                 y_test = y_test.reset_index(drop=True)
 
-                # Transformamos todos a numpy para poder trabajas con ellos más adelante
                 X_training = X_training.to_numpy()
                 y_training = y_training.to_numpy()
                 X_test = X_test.to_numpy()
                 y_test = y_test.to_numpy()
 
                 return X_training, y_training, X_test, y_test
       '''
@@ -163,24 +158,22 @@
 def forwd1():
     string = '''
             def forward(theta1, theta2, theta3, X):
                 #Variables necesarias
                 m = len(X)
                 ones = np.ones((m, 1))
 
-                #Calculamos las activaciones añadiendole la bias después
                 a1 = np.hstack((ones, X))
 
                 a2 = sigmoid(a1 @ theta1.T)
                 a2 = np.hstack((ones, a2))
 
                 a3 = sigmoid(a2 @ theta2.T)
                 a3 = np.hstack((ones, a3))
 
-                #a4 es la hipótesis y no necesitará la bias
                 a4 = sigmoid(a3 @ theta3.T)
 
                 return a1, a2, a3, a4
       '''
 
     print(string)
 
@@ -191,43 +184,32 @@
             nn_params = np.hstack((theta1.ravel(order='F'), theta2.ravel(order='F'), theta3.ravel(order='F')))
             J = nnCostFunction(nn_params, input_layer_size, hidden_layer_size1, hidden_layer_size2, num_labels, X_training,
                        y_training)
 
             # Funcion
             def nnCostFunction(nn_params, input_layer_size, hidden_layer_size1, hidden_layer_size2, num_labels, X, y):
 
-                #Variable útil más adelante
                 m = len(X)
-
-                #Obtenemos las thetas:
                 inicio = 0
                 fin = hidden_layer_size1 * (input_layer_size+1)
                 theta1 = np.reshape(a=nn_params[inicio:fin], newshape=(hidden_layer_size1, input_layer_size+1), order='F')
                 inicio = fin
                 fin = fin + (hidden_layer_size2*(hidden_layer_size1+1))
                 theta2 = np.reshape(a=nn_params[inicio:fin], newshape=(hidden_layer_size2, hidden_layer_size1+1), order='F')
                 inicio = fin
                 theta3 = np.reshape(a=nn_params[inicio:], newshape=(num_labels, hidden_layer_size2+1), order='F')
 
-                #Obtenemos la hipótesis con la última activación que nos da el forward
                 a1, a2, a3, h = forward(theta1,theta2,theta3,X)
 
-                #Transformamos y en el DataFrame por columnas que necesitamos
-                #y = y.to_numpy()
                 y_d = pd.get_dummies(y.flatten())
 
-                #Calculamos el coste
-                #Para cuando y=1
                 temp1 = np.multiply(y_d, np.log(h))
-                #Para cuando y=0
                 temp2 = np.multiply(1-y_d, np.log(1-h))
-                #Suma de ambas
                 temp3 = np.sum(temp1 + temp2)
 
-                #Coste final
                 J = - np.sum(temp3) / m
 
                 return J
       '''
 
     print(string)
 
@@ -236,39 +218,31 @@
     string = '''
             # Main
             lambda_param = 0
             checkNNGradients(lambda_param)
 
             # Funcion
             def nnGradFunction(nn_params, input_layer_size, hidden_layer_size1, hidden_layer_size2, num_labels, X, y):
-                #Obtenemos las thetas:
                 inicio = 0
                 fin = hidden_layer_size1 * (input_layer_size+1)
                 initial_theta1 = np.reshape(a=nn_params[inicio:fin], newshape=(hidden_layer_size1, input_layer_size+1), order='F')
                 inicio = fin
                 fin = fin + (hidden_layer_size2*(hidden_layer_size1+1))
                 initial_theta2 = np.reshape(a=nn_params[inicio:fin], newshape=(hidden_layer_size2, hidden_layer_size1+1), order='F')
                 inicio = fin
                 initial_theta3 = np.reshape(a=nn_params[inicio:], newshape=(num_labels, hidden_layer_size2+1), order='F')
 
-                #Variables útiles:
                 m = len(y)
-
-                #y = y.to_numpy()
                 y_d = pd.get_dummies(y.flatten())
 
                 a1, a2, a3, a4 = forward(initial_theta1,initial_theta2, initial_theta3, X)
 
-                #Obtenemos las delta minúscula
                 d4 = a4 - y_d
-
                 d3 = np.multiply(np.dot(d4, initial_theta3), np.multiply(a3, 1-a3))
                 d2 = np.multiply(np.dot(d3[:,1:], initial_theta2), np.multiply(a2, 1 - a2))
-
-                #Le quitamos la bias a las delta minúscula para poder calcular las Delta mayúscula
                 d3 = d3[:,1:]
                 d2 = d2[:,1:]
 
 
                 delta1 = d2.T @ a1
                 delta2 = d3.T @ a2
                 delta3 = d4.T @ a3
@@ -323,28 +297,25 @@
               X_test_normal.append(x)
 
             pred = predict(nn_params, input_layer_size, hidden_layer_size1, hidden_layer_size2, num_labels, X_test_normal)
             print("Accuracy del conjunto de test: ", np.mean(pred.flatten() == y_test.flatten()) * 100)
 
             # Funcion
             def predict(nn_params, input_layer_size, hidden_layer_size1, hidden_layer_size2, num_labels, X):
-                # Obtenemos las thetas
                 inicio = 0
                 fin = hidden_layer_size1 * (input_layer_size + 1)
                 theta1 = np.reshape(a=nn_params[inicio:fin], newshape=(hidden_layer_size1, input_layer_size + 1), order='F')
                 inicio = fin
                 fin = fin + (hidden_layer_size2 * (hidden_layer_size1 + 1))
                 theta2 = np.reshape(a=nn_params[inicio:fin], newshape=(hidden_layer_size2, hidden_layer_size1 + 1), order='F')
                 inicio = fin
                 theta3 = np.reshape(a=nn_params[inicio:], newshape=(num_labels, hidden_layer_size2 + 1), order='F')
 
-                # Obtenemos la hipótesis con a4
                 a1, a2, a3, a4 = forward(theta1, theta2, theta3, X)
 
-                # Devolvemos el que más valor tenga en la hipótesis
                 return np.argmax(a4, axis=1)
       '''
     print(string)
 
 
 def carga2():
     string = '''
```

