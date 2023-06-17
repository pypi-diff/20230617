# Comparing `tmp/odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1-py3-none-any.whl.zip` & `tmp/odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,19 @@
-Zip file size: 22670 bytes, number of entries: 14
--rw-r--r--  2.0 unx     2041 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/README.rst
--rw-r--r--  2.0 unx       23 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/__init__.py
--rw-r--r--  2.0 unx      598 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/__manifest__.py
--rw-r--r--  2.0 unx      826 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/i18n/invader_payment_stripe.pot
--rw-r--r--  2.0 unx       42 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx       68 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx       29 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/services/__init__.py
--rw-r--r--  2.0 unx     8935 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/services/payment_stripe.py
--rw-r--r--  2.0 unx    10712 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/static/description/icon.png
--rw-r--r--  2.0 unx    10993 b- defN 23-Jan-19 11:20 odoo/addons/invader_payment_stripe/static/description/index.html
--rw-r--r--  2.0 unx     2689 b- defN 23-Jan-19 11:20 odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-19 11:20 odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jan-19 11:20 odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1575 b- defN 23-Jan-19 11:20 odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/RECORD
-14 files, 38628 bytes uncompressed, 19896 bytes compressed:  48.5%
+Zip file size: 24233 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     2041 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/README.rst
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/__init__.py
+-rw-r--r--  2.0 unx      642 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/__manifest__.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/data/decimal_precision.xml
+-rw-r--r--  2.0 unx     1463 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/i18n/invader_payment_stripe.pot
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/models/__init__.py
+-rw-r--r--  2.0 unx     1041 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/models/invader_payable.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/services/__init__.py
+-rw-r--r--  2.0 unx     8773 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/services/payment_stripe.py
+-rw-r--r--  2.0 unx    10712 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/static/description/icon.png
+-rw-r--r--  2.0 unx    10993 b- defN 23-Jun-17 02:59 odoo/addons/invader_payment_stripe/static/description/index.html
+-rw-r--r--  2.0 unx     2689 b- defN 23-Jun-17 03:00 odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 03:00 odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-17 03:00 odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1918 b- defN 23-Jun-17 03:00 odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/RECORD
+17 files, 40937 bytes uncompressed, 20883 bytes compressed:  49.0%
```

## zipnote {}

```diff
@@ -3,17 +3,26 @@
 
 Filename: odoo/addons/invader_payment_stripe/__init__.py
 Comment: 
 
 Filename: odoo/addons/invader_payment_stripe/__manifest__.py
 Comment: 
 
+Filename: odoo/addons/invader_payment_stripe/data/decimal_precision.xml
+Comment: 
+
 Filename: odoo/addons/invader_payment_stripe/i18n/invader_payment_stripe.pot
 Comment: 
 
+Filename: odoo/addons/invader_payment_stripe/models/__init__.py
+Comment: 
+
+Filename: odoo/addons/invader_payment_stripe/models/invader_payable.py
+Comment: 
+
 Filename: odoo/addons/invader_payment_stripe/readme/CONTRIBUTORS.rst
 Comment: 
 
 Filename: odoo/addons/invader_payment_stripe/readme/DESCRIPTION.rst
 Comment: 
 
 Filename: odoo/addons/invader_payment_stripe/services/__init__.py
@@ -24,20 +33,20 @@
 
 Filename: odoo/addons/invader_payment_stripe/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/invader_payment_stripe/static/description/index.html
 Comment: 
 
-Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/METADATA
+Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/WHEEL
+Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/top_level.txt
+Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/RECORD
+Filename: odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/invader_payment_stripe/__init__.py

```diff
@@ -1 +1,2 @@
+from . import models
 from . import services
```

## odoo/addons/invader_payment_stripe/__manifest__.py

```diff
@@ -1,15 +1,16 @@
 # Copyright 2019 ACSONE SA/NV (http://acsone.eu).
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 {
     "name": "Stripe Payment Acquirer (REST, Base)",
     "summary": "REST Services for Stripe Payments (base module)",
-    "version": "14.0.1.0.1",
+    "version": "14.0.1.0.2",
     "category": "e-commerce",
     "website": "https://github.com/shopinvader/odoo-shopinvader-payment",
     "author": "ACSONE SA/NV",
     "license": "AGPL-3",
     "external_dependencies": {"python": ["cerberus", "stripe"], "bin": []},
     "depends": ["invader_payment", "payment_stripe", "base_rest"],
+    "data": ["data/decimal_precision.xml"],
     "installable": True,
 }
```

## odoo/addons/invader_payment_stripe/i18n/invader_payment_stripe.pot

```diff
@@ -10,20 +10,40 @@
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
 
 #. module: invader_payment_stripe
+#: model:ir.model,name:invader_payment_stripe.model_invader_payable
+msgid "Adyen Klarna capture Mixin"
+msgstr ""
+
+#. module: invader_payment_stripe
+#: model:ir.model.fields,field_description:invader_payment_stripe.field_invader_payable__display_name
+msgid "Display Name"
+msgstr ""
+
+#. module: invader_payment_stripe
 #: code:addons/invader_payment_stripe/services/payment_stripe.py:0
 #, python-format
 msgid "Exception: {}"
 msgstr ""
 
 #. module: invader_payment_stripe
+#: model:ir.model.fields,field_description:invader_payment_stripe.field_invader_payable__id
+msgid "ID"
+msgstr ""
+
+#. module: invader_payment_stripe
+#: model:ir.model.fields,field_description:invader_payment_stripe.field_invader_payable____last_update
+msgid "Last Modified on"
+msgstr ""
+
+#. module: invader_payment_stripe
 #: code:addons/invader_payment_stripe/services/payment_stripe.py:0
 #, python-format
 msgid "Payment Error"
 msgstr ""
 
 #. module: invader_payment_stripe
 #: code:addons/invader_payment_stripe/services/payment_stripe.py:0
```

## odoo/addons/invader_payment_stripe/services/payment_stripe.py

```diff
@@ -3,19 +3,17 @@
 
 import logging
 
 import stripe
 from cerberus import Validator
 
 from odoo import _
-from odoo.tools.float_utils import float_round
 
 from odoo.addons.base_rest.components.service import to_int
 from odoo.addons.component.core import AbstractComponent
-from odoo.addons.payment_stripe.models.payment import INT_CURRENCIES
 
 _logger = logging.getLogger(__name__)
 
 # map Stripe transaction statuses to Odoo payment.transaction statuses
 STRIPE_TRANSACTION_STATUSES = {
     "canceled": "cancel",
     "processing": "pending",
@@ -69,26 +67,23 @@
                 "payment_intent_client_secret": {"type": "string"},
                 "success": {"type": "boolean"},
                 "error": {"type": "string"},
             },
             allow_unknown=True,
         )
 
-    def _get_formatted_amount(self, currency, amount):
+    def _get_formatted_amount(self, transaction, amount):
         """
         The expected amount format by Stripe
         :param amount: float
         :return: int
         """
-        res = int(
-            amount
-            if currency.name in INT_CURRENCIES
-            else float_round(amount * 100, 2)
+        return self.env["invader.payable"]._get_formatted_amount(
+            transaction, amount
         )
-        return res
 
     def _get_stripe_transaction_from_intent(self, intent):
         """
         Retrieve the transaction from intent string
         :param intent: string
         :return: payment.transaction
         """
@@ -191,15 +186,15 @@
         :param stripe_payment_method_id:
         :return: StripeIntent
         """
         metadata = {"reference": transaction.reference}
         currency = transaction.currency_id
         intent = stripe.PaymentIntent.create(
             payment_method=stripe_payment_method_id,
-            amount=self._get_formatted_amount(currency, transaction.amount),
+            amount=self._get_formatted_amount(transaction, transaction.amount),
             currency=currency.name,
             confirmation_method="manual",
             confirm=True,
             description=transaction.reference,
             metadata=metadata,
             api_key=self._get_stripe_private_key(transaction),
         )
```

## Comparing `odoo14_addon_invader_payment_stripe-14.0.1.0.2.dev1.dist-info/METADATA` & `odoo14_addon_invader_payment_stripe-14.0.1.0.3.dev1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-invader-payment-stripe
-Version: 14.0.1.0.2.dev1
+Version: 14.0.1.0.3.dev1
 Summary: REST Services for Stripe Payments (base module)
 Home-page: https://github.com/shopinvader/odoo-shopinvader-payment
 Author: ACSONE SA/NV
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

