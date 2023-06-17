# Comparing `tmp/kodexam-0.0.1.tar.gz` & `tmp/kodexam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexam-0.0.1.tar", last modified: Fri Jun 16 23:48:12 2023, max compression
+gzip compressed data, was "kodexam-0.0.2.tar", last modified: Sat Jun 17 00:04:09 2023, max compression
```

## Comparing `kodexam-0.0.1.tar` & `kodexam-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:48:12.785646 kodexam-0.0.1/
--rw-rw-rw-   0        0        0      108 2023-06-16 23:19:25.000000 kodexam-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-06-16 23:20:19.000000 kodexam-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       27 2023-06-16 23:38:22.000000 kodexam-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      646 2023-06-16 23:48:12.785646 kodexam-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-16 23:17:20.000000 kodexam-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 23:48:12.780660 kodexam-0.0.1/kodexam/
--rw-rw-rw-   0        0        0   190214 2023-06-16 23:03:03.000000 kodexam-0.0.1/kodexam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:48:12.784649 kodexam-0.0.1/kodexam.egg-info/
--rw-rw-rw-   0        0        0      646 2023-06-16 23:48:12.000000 kodexam-0.0.1/kodexam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-16 23:48:12.000000 kodexam-0.0.1/kodexam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:48:12.000000 kodexam-0.0.1/kodexam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 23:48:12.000000 kodexam-0.0.1/kodexam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 23:48:12.785646 kodexam-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-16 23:47:56.000000 kodexam-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:04:09.707610 kodexam-0.0.2/
+-rw-rw-rw-   0        0        0      108 2023-06-16 23:19:25.000000 kodexam-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-06-16 23:20:19.000000 kodexam-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       27 2023-06-16 23:38:22.000000 kodexam-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      646 2023-06-17 00:04:09.707610 kodexam-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-16 23:17:20.000000 kodexam-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 00:04:09.703098 kodexam-0.0.2/kodexam/
+-rw-rw-rw-   0        0        0   190238 2023-06-17 00:01:57.000000 kodexam-0.0.2/kodexam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 00:04:09.706598 kodexam-0.0.2/kodexam.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-06-17 00:04:09.000000 kodexam-0.0.2/kodexam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-17 00:04:09.000000 kodexam-0.0.2/kodexam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 00:04:09.000000 kodexam-0.0.2/kodexam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 00:04:09.000000 kodexam-0.0.2/kodexam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 00:04:09.707610 kodexam-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-17 00:03:27.000000 kodexam-0.0.2/setup.py
```

### Comparing `kodexam-0.0.1/LICENSE.txt` & `kodexam-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kodexam-0.0.1/PKG-INFO` & `kodexam-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexam
-Version: 0.0.1
+Version: 0.0.2
 Summary: Very useful thing
 Home-page: 
 Author: Dimasik
 Author-email: drobyshevskiydk@gmail.com
 License: MIT
 Keywords: kod
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kodexam-0.0.1/kodexam/__init__.py` & `kodexam-0.0.2/kodexam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1143,15 +1143,15 @@
 @tol(5, 0)  # Декоратор с параметрами len=5 и fill=0\n\
 def generate_sequence():\n\
     return [1, 2, 3]\n\
 result = generate_sequence()\n\
 print(result)'
             ,
 #32
-            'Реализовать однонаправленный связанный':'Реализовать однонаправленный связанный список (реализовать класс для элементов списка). Преобразовать строку «Eeny, meeny, miney, moe; Catch a tiger by his toe.» в связный список символов строки и удалить из него все элементы содержащие гласные буквы.\n\
+                        'Реализовать однонаправленный связанный':'Реализовать однонаправленный связанный список (реализовать класс для элементов списка). Преобразовать строку «Eeny, meeny, miney, moe; Catch a tiger by his toe.» в связный список символов строки и удалить из него все элементы содержащие гласные буквы.\n\
 \n\
 class Node:\n\
     def __init__(self, data):\n\
         self.data = data\n\
         self.next = None\n\
 class LinkedList:\n\
     def __init__(self):\n\
@@ -1184,22 +1184,22 @@
     def display(self):\n\
         current = self.head\n\
         while current:\n\
             print(current.data, end=" ")\n\
             current = current.next\n\
         print()\n\
 # Создание связанного списка из строки\n\
-string = "Eeny, meeny, miney, moe; Catch a tiger by his toe."\n\
+string = «Eeny, meeny, miney, moe; Catch a tiger by his toe.»\n\
 linked_list = LinkedList()\n\
 for char in string:\n\
     linked_list.insert(char)\n\
 # Удаление элементов с гласными буквами\n\
 linked_list.remove_vowels()\n\
 # Вывод связанного списка\n\
-linked_list.display()\n\'
+linked_list.display()'
             ,
 #33
             'Создать базовый класс':'Создать базовый класс по следующей предметной области. Известны оклад (зарплата) и ставка процента подоходного налога. Определить размер подоходного налога и сумму, получаемую на руки. Исходными данными являются величина оклада (переменная oklad, выражаемая числом) и ставка подоходного налога (переменная procent, выражаемая числом). Размер налога (переменная nalog) определяется как oklad∗procent/100, а сумма, получаемая на руки (переменная summa) — как oklad-nalog. \n\
 \n\
 class Salary:\n\
     def __init__(self, oklad, procent):\n\
         self.oklad = oklad\n\
@@ -1302,18 +1302,18 @@
     def __init__(self, sort, country, weight):\n\
         self.index = Mango.generate_next_index()\n\
         self.sort = sort\n\
         self.country = country\n\
         self.weight = weight\n\
         \n\
     def price(self):\n\
-        return f"the price is {self.weight * 100}"\n\
+        return f»the price is {self.weight * 100}»\n\
     \n\
     def __str__(self):\n\
-        return f"Сорт манго - {self.sort}, страна - {self.country}, вес - {self.weight}"\n\
+        return f»Сорт манго - {self.sort}, страна - {self.country}, вес - {self.weight}»\n\
 \n\
 class Banana(Mango):\n\
     next_index = 0\n\
     \n\
     @classmethod\n\
     def generate_next_index(cls):\n\
         index = cls.next_index\n\
@@ -1341,22 +1341,22 @@
         super().__init__(sort, country, weight)\n\
         self.index = Apple.generate_next_index()\n\
         self.count = count\n\
         \n\
     def price(self):\n\
         return super().price()\n\
         \n\
-a1 = Apple("red", "USA", 2, 3)\n\
+a1 = Apple(«red», «USA», 2, 3)\n\
 a1.next_index\n\
-a2 = Apple("blue", "Kazakhstan", 1, 4)\n\
+a2 = Apple(«blue», «Kazakhstan», 1, 4)\n\
 a2.next_index\n\
-m = Mango("dope", "Brazil", 0.2)\n\
-m1 = Mango("aloa", "Brazil", 0.5)\n\
-m2 = Mango("waergsedrgearg", "Rushka", 123)\n\
-m2.next_index\n\'
+m = Mango(«dope», «Brazil», 0.2)\n\
+m1 = Mango(«aloa», «Brazil», 0.5)\n\
+m2 = Mango(«waergsedrgearg», «Rushka», 123)\n\
+m2.next_index'
             ,
 #38
             'Расположить по алфавиту':'Расположить по алфавиту имена владельцев и, соответственно, вывести информацию об их машинах.  Использовать алгоритм сортировки выбором.\n\
 \n\
 def selection_sort(owners, cars):\n\
     n = len(owners)\n\
     for i in range(n-1):\n\
@@ -1373,15 +1373,15 @@
 cars = ["Toyota", "Ford", "Honda", "BMW"]\n\
 \n\
 # Вызываем сортировку выбором\n\
 selection_sort(owners, cars)\n\
 \n\
 # Выводим информацию об отсортированных владельцах и их машинах\n\
 for i in range(len(owners)):\n\
-    print(f"Владелец: {owners[i]}, Машина: {cars[i]}")\n\'
+    print(f"Владелец: {owners[i]}, Машина: {cars[i]}")'
             ,
 #39
             'Описать рекурсивную функцию':'Описать рекурсивную функцию Root (а, b, ε), которая методом деления отрезка пополам находит с точностью ε корень уравнения f(x) = 0 на отрезке [а, b] (считать, что ε > 0, а < b, f(a) – f(b) < 0 и f(x) — непрерывная и монотонная на отрезке [а, b] функция).\n\
 \n\
 def Root(a, b, ε):\n\
     c = (a + b) / 2  # Находим середину отрезка\n\
     if abs(f(c)) < ε:\n\
@@ -1641,15 +1641,14 @@
         if current1.value == current2.value:\n\
             L3.add(current1.value)\n\
         current2 = current2.next\n\
     current1 = current1.next\n\
 print(L1)\n\
 print(L2)\n\
 print(L3)\n\
-
 '
             ,
 #48
             'Создать класс Профиль':'Создать класс Профиль местности, который хранит последовательность высот, вычисленных через равные промежутки по горизонтали. Методы: наибольшая высота, наименьшая высота, перепад высот (наибольший, суммарный), крутизна (тангенс угла наклона; наибольшая, средняя), сравнение двух профилей одинаковой длины (по перепаду, по крутизне). (20 баллов)\n\
 class Profile:\n\
     def __init__(self, heights):\n\
         self.heights = heights\n\
@@ -1769,15 +1768,15 @@
 r = BinaryNode(5)\n\
 r.set_left_child(7)\n\
 r.set_right_child(6)\n\
 r.get_left_child().set_left_child(10)\n\
 r.get_left_child().set_right_child(30)\n\
 r.set_right_child(20)\n\
 r.__str__()\n\
-in_order(r)\n\'
+in_order(r)'
             ,
 #51-55
             'В одномерном массиве':'В одномерном массиве целых чисел найти количество пар элементов разного знака. (пара — это два рядом стоящих элемента). (20 баллов)\n\
 counter = 0 # счетчик для пар \n\
 array = [1, -1, 2, 4 ,5, -6, 2, 3]\n\
 for i in range(len(array)-1):\n\
     if array[i] < 0 and array[i+1] > 0: # проверка знаков\n\
```

### Comparing `kodexam-0.0.1/kodexam.egg-info/PKG-INFO` & `kodexam-0.0.2/kodexam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexam
-Version: 0.0.1
+Version: 0.0.2
 Summary: Very useful thing
 Home-page: 
 Author: Dimasik
 Author-email: drobyshevskiydk@gmail.com
 License: MIT
 Keywords: kod
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kodexam-0.0.1/setup.py` & `kodexam-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='kodexam',
-    version='0.0.1',
+    version='0.0.2',
     description='Very useful thing',
     long_description=open('README.txt').read()+'\n\n'+open('CHANGELOG.txt').read(),
     url='',
     author='Dimasik',
     author_email='drobyshevskiydk@gmail.com',
     classifiers=classifiers,
     license='MIT',
```

