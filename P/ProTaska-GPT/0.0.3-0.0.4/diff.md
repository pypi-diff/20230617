# Comparing `tmp/ProTaska-GPT-0.0.3.tar.gz` & `tmp/ProTaska-GPT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.3.tar", last modified: Thu Jun 15 21:52:05 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.4.tar", last modified: Sat Jun 17 16:24:43 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.3.tar` & `ProTaska-GPT-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.892230 ProTaska-GPT-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2208 2023-06-15 21:52:05.891220 ProTaska-GPT-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.859976 ProTaska-GPT-0.0.3/ProTaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.3/ProTaska/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.867178 ProTaska-GPT-0.0.3/ProTaska/data/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.3/ProTaska/data/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.3/ProTaska/data/data_utils.py
--rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.3/ProTaska/data/ingestion.py
--rw-rw-rw-   0        0        0     5317 2023-06-15 20:26:22.000000 ProTaska-GPT-0.0.3/ProTaska/data/loader.py
--rw-rw-rw-   0        0        0     1807 2023-06-15 20:19:34.000000 ProTaska-GPT-0.0.3/ProTaska/describer.py
--rw-rw-rw-   0        0        0     1878 2023-06-15 21:11:54.000000 ProTaska-GPT-0.0.3/ProTaska/ideate.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.889220 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0     2208 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1486 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 21:52:05.892230 ProTaska-GPT-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-06-15 21:51:53.000000 ProTaska-GPT-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.903261 ProTaska-GPT-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:24:43.901078 ProTaska-GPT-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.736427 ProTaska-GPT-0.0.4/ProTaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.4/ProTaska/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.800058 ProTaska-GPT-0.0.4/ProTaska/data/
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.4/ProTaska/data/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.4/ProTaska/data/data_utils.py
+-rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.4/ProTaska/data/ingestion.py
+-rw-rw-rw-   0        0        0     5317 2023-06-17 15:32:34.000000 ProTaska-GPT-0.0.4/ProTaska/data/loader.py
+-rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.4/ProTaska/describer.py
+-rw-rw-rw-   0        0        0     3143 2023-06-17 16:18:56.000000 ProTaska-GPT-0.0.4/ProTaska/ideate.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:24:43.889546 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2167 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 16:24:43.000000 ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:24:43.904309 ProTaska-GPT-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2023-06-17 16:24:33.000000 ProTaska-GPT-0.0.4/setup.py
```

### Comparing `ProTaska-GPT-0.0.3/LICENSE` & `ProTaska-GPT-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.3/PKG-INFO` & `ProTaska-GPT-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,17 @@
 
 
 Specify your dataset of choice, and ProTaska-GPT generates a tailored codebase, empowering you to visualize and understand the dataset with tasks, tutorials, and actionable insights. Accelerate your data science journey with ease and efficiency!
 
 ## 🖊️ Key Features:
 
 1. **Dataset Ingestion:** ProTaska-GPT seamlessly integrates with dataset sources like Kaggle and Hugging Face (_for now_), allowing users to easily import and work with diverse datasets.
-2. **Visualize, Inspect, and Understand:** It provides powerful tools to visualize and explore datasets, enabling users to gain insights into data distributions, correlations, missing values, and other important characteristics.
-3. **Task Recommendations:** Leveraging its GPT-backbone, it generates a customized set of tasks tailored to each dataset, providing users with valuable project ideas and challenges.
-4. **Algorithm Suggestions:** Based on the dataset characteristics, it suggests suitable machine learning algorithms, enabling users to make informed decisions during their project journey.
-5. **Beginner-Friendly Tutorials**: ProTaska-GPT offers to generate a collection of beginner-friendly tutorials that guide users through common data science workflows, step-by-step, fostering practical learning and skill development.
+2. **Task Recommendations:** Leveraging its GPT-backbone, it generates a customized set of tasks tailored to each dataset, providing users with valuable project ideas and challenges.
+3. **Algorithm Suggestions:** Based on the dataset characteristics, it suggests suitable machine learning algorithms, enabling users to make informed decisions during their project journey.
+4. **Conversational Chatbot:** Allow user to discuss about different techniques and scrape information from Wikipedia to give relevant responses.
+
+## 🔎 Objectives:
+1. **Beginner-Friendly Tutorials**: ProTaska-GPT aims to offer automated generation of a collection of beginner-friendly tutorials that guide users through common data science workflows, step-by-step, fostering practical learning and skill development.
 
 ## 💁 Contributing
 
 This is an open-source project and we would be really grateful to any contributions.
```

### Comparing `ProTaska-GPT-0.0.3/ProTaska/data/data_utils.py` & `ProTaska-GPT-0.0.4/ProTaska/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.3/ProTaska/data/ingestion.py` & `ProTaska-GPT-0.0.4/ProTaska/data/ingestion.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.3/ProTaska/data/loader.py` & `ProTaska-GPT-0.0.4/ProTaska/data/loader.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.3/ProTaska/describer.py` & `ProTaska-GPT-0.0.4/ProTaska/describer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import argparse
 from .data.loader import HuggingFaceDatasetImporter, LocalDatasetImporter, KaggleDatasetImporter
 from langchain.chat_models import ChatOpenAI
-import gradio as gr
 
-def process_input(openai_key, importer_type, dataset_key=None, destination_path=None):
+def describe_dataset(openai_key, importer_type, destination_path, dataset_key=None,):
     # Process input based on the selected importer
-    llm = ChatOpenAI(model_name="gpt-3.5-turbo",openai_api_key=openai_key,temperature=0)
+    llm = ChatOpenAI(model_name="gpt-3.5-turbo", openai_api_key=openai_key, temperature=0)
     if importer_type == "HuggingFaceDatasetImporter":
         data_ingestor = HuggingFaceDatasetImporter()
         data_ingestor.import_dataset(dataset_key, destination_path)
         data_ingestor.walk_dataset(destination_path)
         out = data_ingestor.ingest(llm=llm)
         return f"Description: {out}"
     elif importer_type == "KaggleDatasetImporter":
@@ -21,22 +21,20 @@
         data_ingestor = LocalDatasetImporter()
         data_ingestor.walk_dataset(destination_path)
         out = data_ingestor.ingest(llm=llm)
         return f"Description: {out}"
     else:
         return "Invalid selection"
 
-iface = gr.Interface(
-    fn=process_input,
-    inputs=[
-        gr.inputs.Textbox(label="OpenAI Key", lines=1),
-        gr.inputs.Dropdown(
-            label="Importer Type",
-            choices=["HuggingFaceDatasetImporter", "KaggleDatasetImporter", "LocalDatasetImporter"]
-        ),
-        gr.inputs.Textbox(label="Dataset Key (Optional)", lines=1),
-        gr.inputs.Textbox(label="Destination Path", lines=1)
-    ],
-    outputs=gr.outputs.Textbox(label="Output")
-)
+def main():
+    parser = argparse.ArgumentParser(description="Menu options for processing input.")
+    parser.add_argument("openai_key", type=str, help="OpenAI Key")
+    parser.add_argument("importer_type", type=str, choices=["HuggingFaceDatasetImporter", "KaggleDatasetImporter", "LocalDatasetImporter"], help="Importer Type")
+    parser.add_argument("--dataset_key", type=str, help="Dataset Key (Optional)")
+    parser.add_argument("destination_path", type=str, help="Destination Path")
+    args = parser.parse_args()
 
-iface.launch()
+    output = describe_dataset(args.openai_key, args.importer_type, args.destination_path, args.dataset_key)
+    print("Output:", output)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ProTaska-GPT-0.0.3/ProTaska/ideate.py` & `ProTaska-GPT-0.0.4/ProTaska/ideate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 from langchain import ConversationChain, LLMChain, PromptTemplate
-from langchain.memory import ConversationBufferWindowMemory
+from langchain.memory import ConversationSummaryBufferMemory 
 from langchain.chat_models import ChatOpenAI
+from langchain.agents import AgentType
+from langchain.agents import initialize_agent
+from langchain.utilities import WikipediaAPIWrapper
+from langchain.tools import Tool
 
+wikipedia = WikipediaAPIWrapper()
+wikipedia.doc_content_chars_max = 3000
 
 template = """ProTaska is a Data Science and Machine Learning expert.
 
 As ProTaska your job is to read the description of a dataset and explore opportunities for data-science. You are to explain the user different forms of ML/DS tasks they can perform if the user hasn't input anything. Each task should be mentioned as points, with a TLDR description of what they may entail.
 
 If the user asks questions you must follow it with responses related to their input query. Remember to be simple and eli5 in your nature of responses.
 
-{history}
 Human: {human_input}
 Assistant:"""
 
 class ChatBotWrapper:
-    def __init__(self, openai_key, dataset_description):
+    def __init__(self, openai_key, dataset_description, agent_verbose=True):
         self.openai_key = openai_key
         self.dataset_description = dataset_description
         self.prompt = PromptTemplate(
-            input_variables=["history", "human_input"], 
+            input_variables=["human_input"], 
             template=template
         )
+        self.llm = ChatOpenAI(model_name="gpt-3.5-turbo",openai_api_key=self.openai_key,temperature=0)
         self.chatgpt_chain = LLMChain(
-            llm=ChatOpenAI(model_name="gpt-3.5-turbo",openai_api_key=self.openai_key,temperature=0), 
+            llm=self.llm,
             prompt=self.prompt, 
             verbose=False, 
-            memory=ConversationBufferWindowMemory(k=2),
         )
         self.first_output = self.chatgpt_chain.predict(human_input="Data Description:\n"+self.dataset_description+'\n')
+        input_string = template.format(human_input="Data Description:\n"+self.dataset_description+'\n')
+        self.memory = ConversationSummaryBufferMemory(llm=self.llm, max_token_limit=200)
+        self.memory.save_context({"input": input_string}, {"output": self.first_output})
+        tools = Tool.from_function(
+            func=wikipedia.run,
+            name="Wikipedia",
+            description="useful for when you need information and sources from Wikipedia!"
+        ),
+        self.agent_chain = initialize_agent(tools=tools, 
+            llm=self.llm, 
+            agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION, 
+            memory=self.memory,
+            verbose=agent_verbose
+        )
+        self.second_output = self.agent_chain.run("Find relevant sources from Wikipedia from the above techniques and advances you just said. Also include some TLDRs in front of those links. Be specific to the ML techniques previously mentioned.")
 
     def __call__(self, human_input):
-        output = self.chatgpt_chain.predict(human_input=human_input)
+        output = self.agent_chain.run(human_input)
         return output
 
-
-
 def main(openai_key, dataset_description):
     chat_bot = ChatBotWrapper(openai_key, dataset_description)
     print("ProTaska:\t", chat_bot.first_output)
+    print("ProTaska-Source:\t", chat_bot.second_output)
+    print()
     while True:
         human_input = input("Human:\t")
-        print("ProTaska:\t", chat_bot(human_input))
+        print("ProTaska:\t", chat_bot(human_input))
+        print()
```

### Comparing `ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/PKG-INFO` & `ProTaska-GPT-0.0.4/ProTaska_GPT.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,17 @@
 
 
 Specify your dataset of choice, and ProTaska-GPT generates a tailored codebase, empowering you to visualize and understand the dataset with tasks, tutorials, and actionable insights. Accelerate your data science journey with ease and efficiency!
 
 ## 🖊️ Key Features:
 
 1. **Dataset Ingestion:** ProTaska-GPT seamlessly integrates with dataset sources like Kaggle and Hugging Face (_for now_), allowing users to easily import and work with diverse datasets.
-2. **Visualize, Inspect, and Understand:** It provides powerful tools to visualize and explore datasets, enabling users to gain insights into data distributions, correlations, missing values, and other important characteristics.
-3. **Task Recommendations:** Leveraging its GPT-backbone, it generates a customized set of tasks tailored to each dataset, providing users with valuable project ideas and challenges.
-4. **Algorithm Suggestions:** Based on the dataset characteristics, it suggests suitable machine learning algorithms, enabling users to make informed decisions during their project journey.
-5. **Beginner-Friendly Tutorials**: ProTaska-GPT offers to generate a collection of beginner-friendly tutorials that guide users through common data science workflows, step-by-step, fostering practical learning and skill development.
+2. **Task Recommendations:** Leveraging its GPT-backbone, it generates a customized set of tasks tailored to each dataset, providing users with valuable project ideas and challenges.
+3. **Algorithm Suggestions:** Based on the dataset characteristics, it suggests suitable machine learning algorithms, enabling users to make informed decisions during their project journey.
+4. **Conversational Chatbot:** Allow user to discuss about different techniques and scrape information from Wikipedia to give relevant responses.
+
+## 🔎 Objectives:
+1. **Beginner-Friendly Tutorials**: ProTaska-GPT aims to offer automated generation of a collection of beginner-friendly tutorials that guide users through common data science workflows, step-by-step, fostering practical learning and skill development.
 
 ## 💁 Contributing
 
 This is an open-source project and we would be really grateful to any contributions.
```

### Comparing `ProTaska-GPT-0.0.3/README.md` & `ProTaska-GPT-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 
 Specify your dataset of choice, and ProTaska-GPT generates a tailored codebase, empowering you to visualize and understand the dataset with tasks, tutorials, and actionable insights. Accelerate your data science journey with ease and efficiency!
 
 ## 🖊️ Key Features:
 
 1. **Dataset Ingestion:** ProTaska-GPT seamlessly integrates with dataset sources like Kaggle and Hugging Face (_for now_), allowing users to easily import and work with diverse datasets.
-2. **Visualize, Inspect, and Understand:** It provides powerful tools to visualize and explore datasets, enabling users to gain insights into data distributions, correlations, missing values, and other important characteristics.
-3. **Task Recommendations:** Leveraging its GPT-backbone, it generates a customized set of tasks tailored to each dataset, providing users with valuable project ideas and challenges.
-4. **Algorithm Suggestions:** Based on the dataset characteristics, it suggests suitable machine learning algorithms, enabling users to make informed decisions during their project journey.
-5. **Beginner-Friendly Tutorials**: ProTaska-GPT offers to generate a collection of beginner-friendly tutorials that guide users through common data science workflows, step-by-step, fostering practical learning and skill development.
+2. **Task Recommendations:** Leveraging its GPT-backbone, it generates a customized set of tasks tailored to each dataset, providing users with valuable project ideas and challenges.
+3. **Algorithm Suggestions:** Based on the dataset characteristics, it suggests suitable machine learning algorithms, enabling users to make informed decisions during their project journey.
+4. **Conversational Chatbot:** Allow user to discuss about different techniques and scrape information from Wikipedia to give relevant responses.
+
+## 🔎 Objectives:
+1. **Beginner-Friendly Tutorials**: ProTaska-GPT aims to offer automated generation of a collection of beginner-friendly tutorials that guide users through common data science workflows, step-by-step, fostering practical learning and skill development.
 
 ## 💁 Contributing
 
 This is an open-source project and we would be really grateful to any contributions.
```

### Comparing `ProTaska-GPT-0.0.3/setup.py` & `ProTaska-GPT-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ProTaska-GPT',
-    version='0.0.3',
+    version='0.0.4',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=find_packages(exclude=["notebooks", "docs"]),
     url='https://github.com/AmanPriyanshu/protaska-gpt',
     install_requires=[
         'langchain',
         'numpy',
         'pandas',
         'colorama',
-        'gradio',
+        'wikipedia',
         'openai',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

