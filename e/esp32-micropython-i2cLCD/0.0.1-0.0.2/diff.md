# Comparing `tmp/esp32_micropython_i2cLCD-0.0.1.tar.gz` & `tmp/esp32_micropython_i2cLCD-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esp32_micropython_i2cLCD-0.0.1.tar", last modified: Fri Jun 16 19:27:46 2023, max compression
+gzip compressed data, was "esp32_micropython_i2cLCD-0.0.2.tar", last modified: Sat Jun 17 17:36:06 2023, max compression
```

## Comparing `esp32_micropython_i2cLCD-0.0.1.tar` & `esp32_micropython_i2cLCD-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 19:27:46.717749 esp32_micropython_i2cLCD-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-16 19:27:46.673640 esp32_micropython_i2cLCD-0.0.1/LCD/
--rw-rw-rw-   0        0        0        0 2023-06-16 18:38:29.000000 esp32_micropython_i2cLCD-0.0.1/LCD/__init__.py
--rw-rw-rw-   0        0        0     3531 2023-06-16 19:08:58.000000 esp32_micropython_i2cLCD-0.0.1/LCD/i2c_lcd.py
--rw-rw-rw-   0        0        0     3286 2023-06-16 19:25:46.000000 esp32_micropython_i2cLCD-0.0.1/LCD/lcd.py
--rw-rw-rw-   0        0        0     9850 2023-06-16 18:40:03.000000 esp32_micropython_i2cLCD-0.0.1/LCD/lcd_api.py
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 esp32_micropython_i2cLCD-0.0.1/LICENCE
--rw-rw-rw-   0        0        0     1759 2023-06-16 19:27:46.717749 esp32_micropython_i2cLCD-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1300 2023-06-16 19:25:46.000000 esp32_micropython_i2cLCD-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 19:27:46.715838 esp32_micropython_i2cLCD-0.0.1/esp32_micropython_i2cLCD.egg-info/
--rw-rw-rw-   0        0        0     1759 2023-06-16 19:27:46.000000 esp32_micropython_i2cLCD-0.0.1/esp32_micropython_i2cLCD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-16 19:27:46.000000 esp32_micropython_i2cLCD-0.0.1/esp32_micropython_i2cLCD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:27:46.000000 esp32_micropython_i2cLCD-0.0.1/esp32_micropython_i2cLCD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-16 19:27:46.000000 esp32_micropython_i2cLCD-0.0.1/esp32_micropython_i2cLCD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 19:27:46.719129 esp32_micropython_i2cLCD-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-06-16 19:26:36.000000 esp32_micropython_i2cLCD-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 17:36:06.334797 esp32_micropython_i2cLCD-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-17 17:36:06.311617 esp32_micropython_i2cLCD-0.0.2/LCD/
+-rw-rw-rw-   0        0        0        0 2023-06-16 18:38:29.000000 esp32_micropython_i2cLCD-0.0.2/LCD/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-06-17 17:21:58.000000 esp32_micropython_i2cLCD-0.0.2/LCD/i2c_lcd.py
+-rw-rw-rw-   0        0        0     4343 2023-06-17 17:34:40.000000 esp32_micropython_i2cLCD-0.0.2/LCD/lcd.py
+-rw-rw-rw-   0        0        0     9652 2023-06-17 17:35:03.000000 esp32_micropython_i2cLCD-0.0.2/LCD/lcd_api.py
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 esp32_micropython_i2cLCD-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0     2016 2023-06-17 17:36:06.334797 esp32_micropython_i2cLCD-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2023-06-17 17:34:18.000000 esp32_micropython_i2cLCD-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 17:36:06.333222 esp32_micropython_i2cLCD-0.0.2/esp32_micropython_i2cLCD.egg-info/
+-rw-rw-rw-   0        0        0     2016 2023-06-17 17:36:05.000000 esp32_micropython_i2cLCD-0.0.2/esp32_micropython_i2cLCD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-17 17:36:05.000000 esp32_micropython_i2cLCD-0.0.2/esp32_micropython_i2cLCD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 17:36:05.000000 esp32_micropython_i2cLCD-0.0.2/esp32_micropython_i2cLCD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-17 17:36:05.000000 esp32_micropython_i2cLCD-0.0.2/esp32_micropython_i2cLCD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 17:36:06.334797 esp32_micropython_i2cLCD-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-06-17 17:35:35.000000 esp32_micropython_i2cLCD-0.0.2/setup.py
```

### Comparing `esp32_micropython_i2cLCD-0.0.1/LCD/i2c_lcd.py` & `esp32_micropython_i2cLCD-0.0.2/LCD/i2c_lcd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 import utime
 import gc
 
-from lcd_api import LcdApi
+from LCD.lcd_api import LcdApi
 from machine import SoftI2C, Pin
 
 # PCF8574 pin definitions
-MASK_RS = 0x01       # P0
-MASK_RW = 0x02       # P1
-MASK_E  = 0x04       # P2
+MASK_RS = 0x01  # P0
+MASK_RW = 0x02  # P1
+MASK_E = 0x04  # P2
 
 SHIFT_BACKLIGHT = 3  # P3
-SHIFT_DATA      = 4  # P4-P7
+SHIFT_DATA = 4  # P4-P7
 
-class I2cLcd(LcdApi):
-    
-    #Implements a HD44780 character LCD connected via PCF8574 on I2C
 
-    def __init__(self, scl, sda, nl=2, nc=16, freq=10000):
-        i2c = SoftI2C(scl=Pin(scl), sda=Pin(sda), freq=10000)
-        i2c_addr = 0x27
-        num_lines = 2
-        num_columns = 16
+class I2cLcd(LcdApi):
 
+    # Implements a HD44780 character LCD connected via PCF8574 on I2C
 
+    def __init__(self, scl, sda, nl, nc, freq=10000):
 
-        self.i2c = i2c
-        self.i2c_addr = i2c_addr
+        self.i2c = SoftI2C(scl=Pin(scl), sda=Pin(sda), freq=10000)
+        self.i2c_addr = 0x27
         self.i2c.writeto(self.i2c_addr, bytes([0]))
-        utime.sleep_ms(20)   # Allow LCD time to powerup
+        utime.sleep_ms(20)  # Allow LCD time to powerup
         # Send reset 3 times
         self.hal_write_init_nibble(self.LCD_FUNCTION_RESET)
-        utime.sleep_ms(5)    # Need to delay at least 4.1 msec
+        utime.sleep_ms(5)  # Need to delay at least 4.1 msec
         self.hal_write_init_nibble(self.LCD_FUNCTION_RESET)
         utime.sleep_ms(1)
         self.hal_write_init_nibble(self.LCD_FUNCTION_RESET)
         utime.sleep_ms(1)
         # Put LCD into 4-bit mode
         self.hal_write_init_nibble(self.LCD_FUNCTION)
         utime.sleep_ms(1)
-        LcdApi.__init__(self, num_lines, num_columns)
+        LcdApi.__init__(self, nl, nc)
         cmd = self.LCD_FUNCTION
-        if num_lines > 1:
+        if nl > 1:
             cmd |= self.LCD_FUNCTION_2LINES
         self.hal_write_command(cmd)
         gc.collect()
 
     def hal_write_init_nibble(self, nibble):
         # Writes an initialization nibble to the LCD.
         # This particular function is only used during initialization.
         byte = ((nibble >> 4) & 0x0f) << SHIFT_DATA
         self.i2c.writeto(self.i2c_addr, bytes([byte | MASK_E]))
         self.i2c.writeto(self.i2c_addr, bytes([byte]))
         gc.collect()
-        
+
     def hal_backlight_on(self):
         # Allows the hal layer to turn the backlight on
         self.i2c.writeto(self.i2c_addr, bytes([1 << SHIFT_BACKLIGHT]))
         gc.collect()
-        
+
     def hal_backlight_off(self):
-        #Allows the hal layer to turn the backlight off
+        # Allows the hal layer to turn the backlight off
         self.i2c.writeto(self.i2c_addr, bytes([0]))
         gc.collect()
-        
+
     def hal_write_command(self, cmd):
         # Write a command to the LCD. Data is latched on the falling edge of E.
         byte = ((self.backlight << SHIFT_BACKLIGHT) |
                 (((cmd >> 4) & 0x0f) << SHIFT_DATA))
         self.i2c.writeto(self.i2c_addr, bytes([byte | MASK_E]))
         self.i2c.writeto(self.i2c_addr, bytes([byte]))
         byte = ((self.backlight << SHIFT_BACKLIGHT) |
@@ -83,11 +78,11 @@
         byte = (MASK_RS |
                 (self.backlight << SHIFT_BACKLIGHT) |
                 (((data >> 4) & 0x0f) << SHIFT_DATA))
         self.i2c.writeto(self.i2c_addr, bytes([byte | MASK_E]))
         self.i2c.writeto(self.i2c_addr, bytes([byte]))
         byte = (MASK_RS |
                 (self.backlight << SHIFT_BACKLIGHT) |
-                ((data & 0x0f) << SHIFT_DATA))      
+                ((data & 0x0f) << SHIFT_DATA))
         self.i2c.writeto(self.i2c_addr, bytes([byte | MASK_E]))
         self.i2c.writeto(self.i2c_addr, bytes([byte]))
         gc.collect()
```

### Comparing `esp32_micropython_i2cLCD-0.0.1/LCD/lcd.py` & `esp32_micropython_i2cLCD-0.0.2/LCD/lcd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,138 @@
 from utime import sleep_ms
-from i2c_lcd import I2cLcd
+from LCD.i2c_lcd import I2cLcd
 from time import sleep
 
+
 class LCD1602():
-    def __init__(self, scl, sda, num_lines=None, num_columns=None, freq=None):
+    def __init__(self, scl, sda, num_lines=2, num_columns=16, freq=None):
         self.hal_backlightvalue = True
         self.posi = None
-        self.txt = None
         self.escolha = []
         self.lcd = I2cLcd(scl, sda, num_lines, num_columns, freq)
+        self.txt = None
+        self.txtprincipal = None
+        self.posicao = None
 
     def clear(self):
-        self.posi = None
         self.txt = None
+        self.txtprincipal = None
+        self.posi = None
+        self.posicao = None
         self.escolha = []
         self.lcd.clear()
 
     def puts(self, txt, x=0, y=0, desactive_auto=True, moveto=None):
-        return self.lcd.puts(txt,x,y, desactive_auto, moveto)
+        return self.lcd.puts(txt, x, y, desactive_auto, moveto)
 
     def list_to_txt(self):
         lista = []
         for i in self.txt:
             for it in i:
                 if len(it) > 16:
-                    x=1
+                    x = 1
                     st = ''
-                    for i in it:
+                    for char in it:
                         if len(st) == 16:
                             lista.append(st)
                             st = ''
-                        st += i
-                        x+=1
+                        st += char
+                        x += 1
                     if len(st) > 0:
                         lista.append(st)
                 else:
                     lista.append(it)
         self.txt = lista
 
     def notlist_to_txt(self):
         lista = []
         st = ''
-        for i in self.txt:
-            if i == '\n':
+        x = 1
+        for char in self.txt:
+            print(char)
+            if char == '\n':
+                if st != '':
+                    lista.append(st)
+                    st = ''
                 lista.append('')
             else:
                 if len(st) < 16:
-                    st += i
+                    st += char
                 else:
-                   lista.append(st)
-                   st = i
+                    lista.append(st)
+                    st = char
+            if len(self.txt) == x and len(st) < 16:
+                lista.append(st)
+            x += 1
         if len(lista) == 1:
             lista.append('')
+        print(lista)
         self.txt = lista
 
-
     def println(self, txt=None, linha=1):
-        if txt:
+        if txt is not None:
             self.txt = txt
-        if type(txt) == str:
-            self.notlist_to_txt()
-        elif txt(txt) == list:
-            self.list_to_txt()
-        numlinhas = len(self.txt)-2
+            if isinstance(txt, str):
+                self.notlist_to_txt()
+            elif isinstance(txt, list):
+                self.list_to_txt()
+        elif self.txt is None:
+            self.txt = [''] * 2
+
+        numlinhas = len(self.txt) - 1
+
         if linha > numlinhas:
             linha = numlinhas
-        elif linha < -1:
+        elif linha < 0:
             linha = 0
-        self.putsln([self.txt[linha]+" "*(16-len(self.txt[linha])), self.txt[linha-1]+" "*(16-len(self.txt[linha-1]))])
+
+        self.putsln([self.txt[linha - 1] + " " * (16 - len(self.txt[linha - 1])),
+                     self.txt[linha] + " " * (16 - len(self.txt[linha - 1]))])
         sleep_ms(3)
 
     def putsln(self, txt):
         if txt:
-            self.clear()
-            self.puts(txt[0])
-            self.puts(txt[1],0,1)
+            self.puts(txt[0] + " " * (16 - len(txt[0])))
+            self.puts(txt[1] + " " * (16 - len(txt[1])), 0, 1)
 
     def posicao(self, value=None):
         if value:
             self.posi = value
         else:
             return self.posi
 
-    def escolhas(self, txtprincipal, posicao, escolhas=None, select=None):
-        self.puts(txtprincipal+" "*(16-len(txtprincipal)))
+    def apagarlinha(self, y):
+        self.lcd.apagar_linha(y)
+
+    def brilhe(self, n=True, local=None):
+        self.lcd.brilhe(n, local)
+
+    def escolhas(self, txtprincipal=None, posicao=None, escolhas=None, select=None):
+        if posicao:
+            self.posicao = posicao
+        else:
+            if not self.posicao:
+                self.posicao = 0
+
+        if txtprincipal is not None:
+            self.txtprincipal = txtprincipal
+        self.puts(self.txtprincipal + " " * (16 - len(self.txtprincipal)))
         if escolhas:
             self.escolha = escolhas
-        if posicao > len(self.escolha)-1:
-            posicao = 0
-        elif posicao < 0:
-            posicao = len(self.escolha)-1
-        self.puts(str(self.escolhas[posicao])+" " * (16 - len(str(self.escolhas[posicao]))), y=1)
+        if self.posicao > len(self.escolha) - 1:
+            self.posicao = 0
+        elif self.posicao < 0:
+            self.posicao = len(self.escolha) - 1
+        self.puts(str(self.escolha[self.posicao]) + " " * (16 - len(str(self.escolha[self.posicao]))), y=1)
         if select:
+            re = self.escolha[self.posicao]
             self.clear()
-            return self.escolhas[posicao]
+            return re
 
-    def char(self,location, charmap):
+    def char(self, location, charmap):
         self.lcd.custom_char(location, charmap)
 
     def hal_backlight(self):
         self.hal_backlightvalue = not self.hal_backlightvalue
         if self.hal_backlightvalue:
             self.lcd.hal_backlight_on()
         else:
```

### Comparing `esp32_micropython_i2cLCD-0.0.1/LCD/lcd_api.py` & `esp32_micropython_i2cLCD-0.0.2/LCD/lcd_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import time
 
+
 class LcdApi:
-    
     # Implements the API for talking with HD44780 compatible character LCDs.
     # This class only knows what commands to send to the LCD, and not how to get
     # them to the LCD.
     #
     # It is expected that a derived class will implement the hal_xxx functions.
     #
     # The following constant names were lifted from the avrlib lcd.h header file,
     # with bit numbers changed to bit masks.
-    
+
     # HD44780 LCD controller command set
-    LCD_CLR             = 0x01  # DB0: clear display
-    LCD_HOME            = 0x02  # DB1: return to home position
+    LCD_CLR = 0x01  # DB0: clear display
+    LCD_HOME = 0x02  # DB1: return to home position
 
-    LCD_ENTRY_MODE      = 0x04  # DB2: set entry mode
-    LCD_ENTRY_INC       = 0x02  # DB1: increment
-    LCD_ENTRY_SHIFT     = 0x01  # DB0: shift
-
-    LCD_ON_CTRL         = 0x08  # DB3: turn lcd/cursor on
-    LCD_ON_DISPLAY      = 0x04  # DB2: turn display on
-    LCD_ON_CURSOR       = 0x02  # DB1: turn cursor on
-    LCD_ON_BLINK        = 0x01  # DB0: blinking cursor
-
-    LCD_MOVE            = 0x10  # DB4: move cursor/display
-    LCD_MOVE_DISP       = 0x08  # DB3: move display (0-> move cursor)
-    LCD_MOVE_RIGHT      = 0x04  # DB2: move right (0-> left)
+    LCD_ENTRY_MODE = 0x04  # DB2: set entry mode
+    LCD_ENTRY_INC = 0x02  # DB1: increment
+    LCD_ENTRY_SHIFT = 0x01  # DB0: shift
+
+    LCD_ON_CTRL = 0x08  # DB3: turn lcd/cursor on
+    LCD_ON_DISPLAY = 0x04  # DB2: turn display on
+    LCD_ON_CURSOR = 0x02  # DB1: turn cursor on
+    LCD_ON_BLINK = 0x01  # DB0: blinking cursor
+
+    LCD_MOVE = 0x10  # DB4: move cursor/display
+    LCD_MOVE_DISP = 0x08  # DB3: move display (0-> move cursor)
+    LCD_MOVE_RIGHT = 0x04  # DB2: move right (0-> left)
 
-    LCD_FUNCTION        = 0x20  # DB5: function set
-    LCD_FUNCTION_8BIT   = 0x10  # DB4: set 8BIT mode (0->4BIT mode)
+    LCD_FUNCTION = 0x20  # DB5: function set
+    LCD_FUNCTION_8BIT = 0x10  # DB4: set 8BIT mode (0->4BIT mode)
     LCD_FUNCTION_2LINES = 0x08  # DB3: two lines (0->one line)
     LCD_FUNCTION_10DOTS = 0x04  # DB2: 5x10 font (0->5x7 font)
-    LCD_FUNCTION_RESET  = 0x30  # See "Initializing by Instruction" section
+    LCD_FUNCTION_RESET = 0x30  # See "Initializing by Instruction" section
 
-    LCD_CGRAM           = 0x40  # DB6: set CG RAM address
-    LCD_DDRAM           = 0x80  # DB7: set DD RAM address
+    LCD_CGRAM = 0x40  # DB6: set CG RAM address
+    LCD_DDRAM = 0x80  # DB7: set DD RAM address
 
-    LCD_RS_CMD          = 0
-    LCD_RS_DATA         = 1
+    LCD_RS_CMD = 0
+    LCD_RS_DATA = 1
 
-    LCD_RW_WRITE        = 0
-    LCD_RW_READ         = 1
+    LCD_RW_WRITE = 0
+    LCD_RW_READ = 1
 
     def __init__(self, num_lines, num_columns):
         self.num_lines = num_lines
         if self.num_lines > 4:
             self.num_lines = 4
         self.num_columns = num_columns
         if self.num_columns > 40:
@@ -86,20 +86,21 @@
         self.estabrilhando = True
         self.hal_write_command(self.LCD_ON_CTRL | self.LCD_ON_DISPLAY | self.LCD_ON_BLINK)
 
     def blink_cursor_off(self):
         self.estabrilhando = False
         # Turns on the cursor, and makes it no blink (i.e. be solid)
         self.hal_write_command(self.LCD_ON_CTRL | self.LCD_ON_DISPLAY)
-    
+
     def cursor_and_blink(self):
         self.estabrilhando = True
         self.estaaparecendoocurso = True
-        self.hal_write_command(self.LCD_ON_CTRL | self.LCD_ON_DISPLAY | self.LCD_ON_BLINK|
+        self.hal_write_command(self.LCD_ON_CTRL | self.LCD_ON_DISPLAY | self.LCD_ON_BLINK |
                                self.LCD_ON_CURSOR)
+
     def cursor_and_blink_off(self):
         self.estabrilhando = False
         self.estaaparecendoocurso = False
         self.hal_write_command(self.LCD_ON_CTRL | self.LCD_ON_DISPLAY)
 
     def display_on(self):
         # Turns on (i.e. unblanks) the LCD
@@ -107,15 +108,15 @@
 
     def display_off(self):
         # Turns off (i.e. blanks) the LCD
         self.hal_write_command(self.LCD_ON_CTRL)
 
     def backlight_on(self):
         # Turns the backlight on.
-        
+
         # This isn't really an LCD command, but some modules have backlight
         # controls, so this allows the hal to pass through the command.
         self.backlight = True
         self.hal_backlight_on()
 
     def backlight_off(self):
         # Turns the backlight off.
@@ -128,16 +129,16 @@
     def move_to(self, cursor_x, cursor_y):
         # Moves the cursor position to the indicated position. The cursor
         # position is zero based (i.e. cursor_x == 0 indicates first column).
         self.cursor_x = cursor_x
         self.cursor_y = cursor_y
         addr = cursor_x & 0x3f
         if cursor_y & 1:
-            addr += 0x40    # Lines 1 & 3 add 0x40
-        if cursor_y & 2:    # Lines 2 & 3 add number of columns
+            addr += 0x40  # Lines 1 & 3 add 0x40
+        if cursor_y & 2:  # Lines 2 & 3 add number of columns
             addr += self.num_columns
         self.hal_write_command(self.LCD_DDRAM | addr)
 
     def putchar(self, char):
         # Writes the indicated character to the LCD at the current cursor
         # position, and advances the cursor by one position.
         if char == '\n':
@@ -194,16 +195,15 @@
         # Write data to the LCD.
         # It is expected that a derived HAL class will implement this function.
         raise NotImplementedError
 
     def hal_sleep_us(self, usecs):
         # Sleep for some time (given in microseconds)
         time.sleep_us(usecs)
-    
-    
+
     def puts(self, txt, x=0, y=0, desactive_auto=True, moveto=None):
         if desactive_auto:
             estavabrilhando = False
             estavaaparecendoocurso = False
             if self.estabrilhando and self.estaaparecendoocurso:
                 self.cursor_and_blink_off()
                 estavaaparecendoocurso = True
@@ -232,25 +232,25 @@
                 self.cursor_and_blink()
             else:
                 if estavabrilhando:
                     self.blink_cursor_on()
                 if estavaaparecendoocurso:
                     self.show_cursor()
         return True
-                
+
     def brilhe(self, n=True, local=None):
         if local:
             self.move_to(local[0], local[1])
         if n:
             self.cursor_and_blink()
         else:
             self.cursor_and_blink_off()
         return True
-    
-    def apagar_linha(self,y):
+
+    def apagar_linha(self, y):
         self.cursor_and_blink_off()
         self.show_cursor()
         self.cursor_x = 0
         self.cursor_y = y
         self.move_to(self.cursor_x, self.cursor_y)
         txt = '                '
         for i in txt:
```

### Comparing `esp32_micropython_i2cLCD-0.0.1/LICENCE` & `esp32_micropython_i2cLCD-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `esp32_micropython_i2cLCD-0.0.1/PKG-INFO` & `esp32_micropython_i2cLCD-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp32_micropython_i2cLCD
-Version: 0.0.1
+Version: 0.0.2
 Summary: uma biblioteca para utilização de um display i2c no esp32 micropython
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: esp32 micropython i2c LCD
 Platform: UNKNOWN
@@ -53,45 +53,59 @@
         x+=1
 
 print choices
 
     from time import sleep
     
     LCD.escolhas('txtprincipal', 0, ['1','2','3','4','5'])
-
+    
     x = 1
     while True:
         sleep(1)
         LCD.escolhas(posicao=x)
-        x+=1
         if x == 3:
-            print(LCD.escolhas(posicao=x,select=True))
+            print(LCD.escolhas(select=True))
             break
+        x+=1
 
 lcd clear
 
     LCD.clear()
     
 lcd print in line
 
     LCD.putsln(['line 0', 'line 1'])
 
 especial char
 
     from time import sleep
     
-    b = bytearray([...])
-    LCD.char(0,b)    
-    LCD.println(['1','2','3','4',char(0)])
+    b = bytearray([0x04,0x0A,0x04,0x0A,0x04,0x0A,0x04,0x0A])
+    
+    LCD.char(0,b)
+    
+    v = ' 1 \n 2 \n 3 \n 4 \n 5 \n '+chr(0)
+    # or v = ['1','2','3','4','5',chr(0)]
+    
+    LCD.println(v)
     
     x = 2
     while True:
         sleep(1)
         LCD.println(linha=x)
         x+=1
 
     #linha == line for txt(list)
 
 lcd hal backlight
 
     LCD.hal_backlight()
 
+lcd blink
+
+    LCD.brilhe(local=[1,1])
+    # or lcd not blink LCD.brilhe(False) 
+
+lcd animation for clear line
+    
+    LCD.apagarlinha(1)
+
```

### Comparing `esp32_micropython_i2cLCD-0.0.1/README.md` & `esp32_micropython_i2cLCD-0.0.2/esp32_micropython_i2cLCD.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,111 @@
-# I2C LCD micropython esp32
-
-import
-
-    from LCD.lcd import LCD1602
-    
-    LCD = LCD1602(scl=12, sda=14)
-    #LCD1602(scl, sda, num_lines=None, num_columns=None, freq=None):
-
-print
-    
-    LCD.puts('teste',x=0,y=1)
-    #y 0~1
-    #x 0~15
-
-print txt
-
-    from time import sleep
-    
-    LCD.println(['1','2','3','4','5'])
-    
-    x = 2
-    while True:
-        sleep(1)
-        LCD.println(linha=x)
-        x+=1
-
-    #linha == line for txt(list)
-
-for txt
-
-    from time import sleep
-    
-    LCD.println('1 \n 2 \n 3 \n 4 \n 5')
-
-    x = 2
-    while True:
-        sleep(1)
-        LCD.println(linha=x)
-        x+=1
-
-print choices
-
-    from time import sleep
-    
-    LCD.escolhas('txtprincipal', 0, ['1','2','3','4','5'])
-
-    x = 1
-    while True:
-        sleep(1)
-        LCD.escolhas(posicao=x)
-        x+=1
-        if x == 3:
-            print(LCD.escolhas(posicao=x,select=True))
-            break
-
-lcd clear
-
-    LCD.clear()
-    
-lcd print in line
-
-    LCD.putsln(['line 0', 'line 1'])
-
-especial char
-
-    from time import sleep
-    
-    b = bytearray([...])
-    LCD.char(0,b)    
-    LCD.println(['1','2','3','4',char(0)])
-    
-    x = 2
-    while True:
-        sleep(1)
-        LCD.println(linha=x)
-        x+=1
-
-    #linha == line for txt(list)
-
-lcd hal backlight
-
-    LCD.hal_backlight()
+Metadata-Version: 2.1
+Name: esp32-micropython-i2cLCD
+Version: 0.0.2
+Summary: uma biblioteca para utilização de um display i2c no esp32 micropython
+Home-page: UNKNOWN
+Author: issei momonge
+Author-email: mggyggf@gmail.com
+License: MIT License
+Keywords: esp32 micropython i2c LCD
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# I2C LCD micropython esp32
+
+import
+
+    from LCD.lcd import LCD1602
+    
+    LCD = LCD1602(scl=12, sda=14)
+    #LCD1602(scl, sda, num_lines=None, num_columns=None, freq=None):
+
+print
+    
+    LCD.puts('teste',x=0,y=1)
+    #y 0~1
+    #x 0~15
+
+print txt
+
+    from time import sleep
+    
+    LCD.println(['1','2','3','4','5'])
+    
+    x = 2
+    while True:
+        sleep(1)
+        LCD.println(linha=x)
+        x+=1
+
+    #linha == line for txt(list)
+
+for txt
+
+    from time import sleep
+    
+    LCD.println('1 \n 2 \n 3 \n 4 \n 5')
+
+    x = 2
+    while True:
+        sleep(1)
+        LCD.println(linha=x)
+        x+=1
+
+print choices
+
+    from time import sleep
+    
+    LCD.escolhas('txtprincipal', 0, ['1','2','3','4','5'])
+    
+    x = 1
+    while True:
+        sleep(1)
+        LCD.escolhas(posicao=x)
+        if x == 3:
+            print(LCD.escolhas(select=True))
+            break
+        x+=1
+
+lcd clear
+
+    LCD.clear()
+    
+lcd print in line
+
+    LCD.putsln(['line 0', 'line 1'])
+
+especial char
+
+    from time import sleep
+    
+    b = bytearray([0x04,0x0A,0x04,0x0A,0x04,0x0A,0x04,0x0A])
+    
+    LCD.char(0,b)
+    
+    v = ' 1 \n 2 \n 3 \n 4 \n 5 \n '+chr(0)
+    # or v = ['1','2','3','4','5',chr(0)]
+    
+    LCD.println(v)
+    
+    x = 2
+    while True:
+        sleep(1)
+        LCD.println(linha=x)
+        x+=1
+
+    #linha == line for txt(list)
+
+lcd hal backlight
+
+    LCD.hal_backlight()
+
+lcd blink
+
+    LCD.brilhe(local=[1,1])
+    # or lcd not blink LCD.brilhe(False) 
+
+lcd animation for clear line
+    
+    LCD.apagarlinha(1)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

