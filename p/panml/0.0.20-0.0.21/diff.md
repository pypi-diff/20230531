# Comparing `tmp/panml-0.0.20.tar.gz` & `tmp/panml-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.20.tar", last modified: Mon May 29 09:36:09 2023, max compression
+gzip compressed data, was "panml-0.0.21.tar", last modified: Wed May 31 02:00:54 2023, max compression
```

## Comparing `panml-0.0.20.tar` & `panml-0.0.21.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.283115 panml-0.0.20/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.20/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    10409 2023-05-29 09:36:09.283389 panml-0.0.20/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)     9230 2023-05-29 09:35:44.000000 panml-0.0.20/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.276061 panml-0.0.20/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.20/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3485 2023-05-28 12:46:27.000000 panml-0.0.20/panml/constants.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.278416 panml-0.0.20/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.20/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.278962 panml-0.0.20/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.20/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.20/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.280475 panml-0.0.20/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.20/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    20328 2023-05-29 09:35:44.000000 panml-0.0.20/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    13708 2023-05-28 12:46:27.000000 panml-0.0.20/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.20/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.20/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.277903 panml-0.0.20/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    10409 2023-05-29 09:36:09.000000 panml-0.0.20/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-05-29 09:36:09.000000 panml-0.0.20/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-29 09:36:09.000000 panml-0.0.20/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-29 09:36:09.000000 panml-0.0.20/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-29 09:36:09.000000 panml-0.0.20/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-29 09:36:09.284443 panml-0.0.20/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-05-29 09:35:44.000000 panml-0.0.20/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-29 09:36:09.282122 panml-0.0.20/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.20/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.20/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.519999 panml-0.0.21/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.21/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14582 2023-05-31 02:00:54.520375 panml-0.0.21/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13403 2023-05-31 02:00:28.000000 panml-0.0.21/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.512192 panml-0.0.21/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.21/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3485 2023-05-28 12:46:27.000000 panml-0.0.21/panml/constants.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.515045 panml-0.0.21/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.21/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.515771 panml-0.0.21/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.21/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.21/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.517361 panml-0.0.21/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.21/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    20328 2023-05-29 09:35:44.000000 panml-0.0.21/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13708 2023-05-28 12:46:27.000000 panml-0.0.21/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.21/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.21/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.514649 panml-0.0.21/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14582 2023-05-31 02:00:54.000000 panml-0.0.21/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-05-31 02:00:54.000000 panml-0.0.21/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-31 02:00:54.000000 panml-0.0.21/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-31 02:00:54.000000 panml-0.0.21/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-31 02:00:54.000000 panml-0.0.21/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-31 02:00:54.521770 panml-0.0.21/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-05-31 02:00:28.000000 panml-0.0.21/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-31 02:00:54.518949 panml-0.0.21/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.21/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.21/test/test_VectorEngine.py
```

### Comparing `panml-0.0.20/LICENSE` & `panml-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/PKG-INFO` & `panml-0.0.21/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,22 @@
-Metadata-Version: 2.1
-Name: panml
-Version: 0.0.20
-Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
-Home-page: https://github.com/Pan-ML/panml
-Author: PanML team
-Author-email: teampanml@gmail.com
-License: MIT
-Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
 ## Goal
 This package aims to make analysis and experimentation of generative AI/ML models broadly accessible, by providing a simple and consistent interface to foundation models, and abstract methods to support some of the common use-cases. This includes using smaller, less compute heavy Open Source language models to support the various NLP-based Data Science workflows in the industry. Additionally, we want to empower Data Science projects with the tools to easily productionise custom-built generative models.
 
 
 We are passionate about AI technology and AI safety, and this supports our contribution towards a beneficial outcome in an AI-powered world. Please note this is a work in progress, so very much open for collaboration and contribution. 
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
-- [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
+- [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
 
 ### Current supported foundation models
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
 
@@ -67,14 +41,15 @@
 
 You can support us by contributing to this project, as well as providing feedback and ideas in the [issues](https://github.com/Pan-ML/panml/issues) section. 
 
 We would also appreciate if you can give panml a ⭐ on GitHub, and if it adds value to you, sharing this with others in your network on LinkedIn/Twitter/Medium etc who would also find this useful.
 
 
 ## Installation
+Requirement: Python 3.7+
 ```bash
 pip install panml
 ```
 
 ## Usage
 See [quick start guide](https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide) or detailed examples in the [PanML Wiki](https://github.com/Pan-ML/panml/wiki).
 
@@ -118,33 +93,128 @@
 When set to return token probability and perplexity scores
 ```python
 output = lm.predict(df_test['prompts'], max_length=20, display_probability=True)
 df_output = pd.DataFrame(output) # df_output contains columns: text, probability, perplexity
 ```
 
 ### Using open source models from OpenAI
+*Note: For information on obtaining the OpenAI API key. Please see [OpenAI documentation](https://platform.openai.com/)*
 ```python
 lm = ModelPack(model='text-davinci-003', source='openai', api_key=<your_openai_key>)
 
 df = pd.DataFrame({'input_prompts': [
     'The goal of life is',
     'The goal of work is',
     'The goal of leisure is',
 ]})
 
 output = lm.predict(df['input_prompts'])
+print(output)
 ```
 ```
 [' to live a life of purpose, joy, and fulfillment. To find meaning and purpose in life, it is important to focus on what brings you joy and fulfillment, and to strive to make a positive impact on the world. It is also important to take care of yourself and your relationships, and to be mindful of the choices you make. ',
  ' The goal of this work is to develop a comprehensive understanding of a particular topic or issue, and to use that understanding to create solutions or strategies that can be implemented to address the issue. ',
  ' to provide an enjoyable and fulfilling experience that helps to reduce stress, improve physical and mental health, and promote social interaction. Leisure activities can include anything from physical activities such as sports and outdoor recreation, to creative activities such as art and music, to social activities such as attending events or visiting friends. ']
 ```
 
+### Prompt chain engineering
+For detailed examples, see [prompt chain engineering](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering). <br><br>
+Create model pack from OpenAI model description and API key. <br>
+*Note: For information on obtaining the OpenAI API key. Please see [OpenAI documentation](https://platform.openai.com/)*
+```python
+lm = ModelPack(model='text-davinci-002', source='openai', api_key=<your_openai_key>)
+
+prompts = [
+    {'prepend': 'you are a sports coach'},
+    {'prepend': 'produce a daily exercise plan for one week'},
+    {'prepend': 'summarise to the original question'},
+]
+
+output = lm.predict('What is the best way to live a healthy lifestyle?', prompt_modifier=prompts, max_tokens=600)
+print(output['text'])
+```
+```
+'Assuming you are starting from a sedentary lifestyle, a good goal to aim for is 
+30 minutes of moderate-intensity exercise most days of the week. 
+This could include brisk walking, biking, swimming, or using a elliptical trainer. 
+Start with whatever you feel comfortable with and gradually increase your time and intensity as you get more fit. 
+Remember to warm up and cool down for 5-10 minutes before and after your workout. 
+In addition to aerobic exercise, it is also important to include strength training ...'
+```
+Furthermore, if we want to apply more complex text or NLP treatments in our prompt chain pipeline, whether it is for steering the LLM's behaviour, and/or to apply constraints in the output for quality or risk control, we can write custom Python functions and use them in the prompt pipeline. <br><br> To demonstrate this, we use a simple example where we want to detect certain keywords in the LLM output, and then direct the LLM to refuse answering if any of the specified keywords are caught.
+```python3
+def my_keyword_filter(text):
+    keywords_to_elaborate = ['cooking', 'lifestyle', 'health', 'well-being']
+    keywords_to_refuse = ['politic', 'election', 'hack']
+    text = text.lower()
+    elaborate = [word for word in keywords_to_elaborate if word in text]
+    refuse = [word for word in keywords_to_refuse if word in text]
+    
+    # Set responses based on keywords
+    if len(refuse) == 0:
+        if len(elaborate) > 0:
+            return f"Break into step by step details and explain in more than three sentences: {text}"
+        else:
+            return f"Explain: {text}"
+    else:
+        return "Produce response to politely say I can't answer"
+    
+prompts = [
+    {},
+    {'transform': my_keyword_filter},
+]
+```
+Then using the prompt pipeline in the LLM
+```python3
+lm = ModelPack(model='text-davinci-003', source='openai', api_key=<your_openai_key>)
+
+df = pd.DataFrame({'input_prompts': [
+    'What is the best way to cook steak?',
+    'How to create an exercise plan?',
+    'Who is going to win the US election?',
+    'How to hack a bank?'
+]})
+df['output'] = lm.predict(df['input_prompts'], prompt_modifier=prompts, keep_history=True, max_length=1000)
+```
+```
+Responses:
+
+'1. Preheat a heavy skillet or grill over high heat. 
+2. Season the steak with salt and pepper. 
+3. Add the steak to the hot pan and sear for 1-2 minutes per side. 
+4. Reduce the heat to medium-high and cook for an additional 3-4 minutes per side, or until the steak reaches the desired doneness. 
+5. Let the steak rest for 5 minutes before serving.  This combination of high heat and short cooking 
+time will ensure that the steak is cooked to perfection. The high heat will quickly sear the steak, 
+locking in the juices and flavor, while the short cooking time will prevent the steak from becoming overcooked. 
+The resting period will allow the steak to finish cooking and will also help to keep the steak juicy and tender.'
+
+'1. Set your goals: Before you start creating your exercise plan, it’s important to set your goals. 
+Think about what you want to achieve and why. Do you want to lose weight, build muscle, 
+or improve your overall fitness? Consider your current fitness level and any health conditions you may have. 
+2. Choose your exercises: Once you’ve set your goals, it’s time to choose the exercises that will help you reach them. 
+Consider the type of exercise you enjoy and the equipment you have available. 
+Research different exercises and create a plan that works for you. 
+3. Create a schedule: Now that you’ve chosen your exercises, 
+it’s time to create a schedule. Decide how often you’ll exercise and for how long. 
+Make sure to include rest days and plan for any potential obstacles. 
+4. Track your progress: As you work through your exercise plan, track your progress. 
+This will help you stay motivated and make adjustments as needed. Keep track of your workouts, how you feel, 
+and any changes in your body. 
+5. Stay consistent: Consistency is key when it comes to exercise. Make sure you stick to your plan 
+and don’t give up. Find ways to stay motivated and reward yourself for your progress.' 
+
+'I'm sorry, I can't answer that.'
+
+'I'm sorry, I can't answer that.'
+
+```
+
 ### Fine tune custom LLM
-For detailed examples, see [fine tuning your LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM). 
+For detailed examples, see [fine tuning your LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM). <br><br>
+Demonstration example:
 ```python
 # Load model
 lm = ModelPack(model='google/flan-t5-base', source='huggingface', model_args={'gpu': True})
 
 # Specify train args
 train_args = {
     'title': 'my_tuned_flan_t5',
@@ -164,47 +234,31 @@
 # Prepare data
 x = df['input_text']
 y = df['target_text']
 
 # Train model
 lm.fit(x, y, train_args, instruct=True)
 ```
-
-### Prompt chain engineering
-For detailed examples, see [prompt chain engineering](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering). <br>
-Create model pack from OpenAI model description and API key.
+In above example, the tuned model is saved in the local directory: *./results/model_my_tuned_flan_t5* <br><br>
+Loading the model from local directory:
 ```python
-lm = ModelPack(model='text-davinci-002', source='openai', api_key=<your_openai_key>)
-
-prompts = [
-    {'prepend': 'you are a sports coach'},
-    {'prepend': 'produce a daily exercise plan for one week'},
-    {'prepend': 'summarise to the original question'},
-]
-
-output = lm.predict('What is the best way to live a healthy lifestyle?', prompt_modifier=prompts, max_tokens=600)
-output['text']
+lm = ModelPack(model='./results/model_my_tuned_flan_t5', source='local)
 ```
-```
-'Assuming you are starting from a sedentary lifestyle, a good goal to aim for is 
-30 minutes of moderate-intensity exercise most days of the week. 
-This could include brisk walking, biking, swimming, or using a elliptical trainer. 
-Start with whatever you feel comfortable with and gradually increase your time and intensity as you get more fit. 
-Remember to warm up and cool down for 5-10 minutes before and after your workout. 
-In addition to aerobic exercise, it is also important to include strength training in your routine. 
-Strength-training not only helps to tone your body, but can also help to reduce your risk of injuries in the future. 
-A simple way to start strength-training is to use your own body weight for resistance. 
-Try doing push-ups, sit-ups, and squats. As you get stronger, you can add weight by using dumbbells or resistance bands. 
-Aim for two to three days of strength-training per week. 
-Finally, be sure to get enough sleep each night. Most adults need 7-8 hours of sleep per night. 
-Getting enough sleep will help your body to recover from your workouts and will also help to reduce stress levels.'
+Saving the model to local directory:
+```python
+# Specify save directory
+lm.save(save_dir='./my_new_model')
+
+# Or if save directory is not provided, the default directory is: "./results/model_<model name>"
+lm.save()
 ```
 
 ### Prompted code generation
-For detailed examples, see [prompted code generation](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation).
+For detailed examples, see [prompted code generation](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation). <br><br>
+Some open source and commercial LLMs are capable of generating code based on prompt instructions. Here, we explore an experimental use-case to have the LLM generate the code for us, while incorporating a custom variable (this variable can also be a pandas dataframe) into the result.
 ```python
 code = lm.predict_code('calculate the fibonacci sequence using input', x=19, 
                        variable_names={'output': 'ans'}, language='python')
 print(code)
 exec(code) # execute code in Python
 print(f'\nAnswer: {ans}')
 ```
@@ -247,9 +301,7 @@
 pip install -r requirements.txt
 ```
 
 ### Running tests
 ```
 python3 -m unittest
 ```
-
-
```

### Comparing `panml-0.0.20/panml/constants.py` & `panml-0.0.21/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/panml/core/clustering/faiss.py` & `panml-0.0.21/panml/core/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/panml/core/llm/huggingface.py` & `panml-0.0.21/panml/core/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/panml/core/llm/openai.py` & `panml-0.0.21/panml/core/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/panml/models.py` & `panml-0.0.21/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/panml/search.py` & `panml-0.0.21/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/panml.egg-info/PKG-INFO` & `panml-0.0.21/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.20
+Version: 0.0.21
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
@@ -33,16 +33,16 @@
 This package aims to make analysis and experimentation of generative AI/ML models broadly accessible, by providing a simple and consistent interface to foundation models, and abstract methods to support some of the common use-cases. This includes using smaller, less compute heavy Open Source language models to support the various NLP-based Data Science workflows in the industry. Additionally, we want to empower Data Science projects with the tools to easily productionise custom-built generative models.
 
 
 We are passionate about AI technology and AI safety, and this supports our contribution towards a beneficial outcome in an AI-powered world. Please note this is a work in progress, so very much open for collaboration and contribution. 
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
-- [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
+- [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
 
 ### Current supported foundation models
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
 
@@ -67,14 +67,15 @@
 
 You can support us by contributing to this project, as well as providing feedback and ideas in the [issues](https://github.com/Pan-ML/panml/issues) section. 
 
 We would also appreciate if you can give panml a ⭐ on GitHub, and if it adds value to you, sharing this with others in your network on LinkedIn/Twitter/Medium etc who would also find this useful.
 
 
 ## Installation
+Requirement: Python 3.7+
 ```bash
 pip install panml
 ```
 
 ## Usage
 See [quick start guide](https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide) or detailed examples in the [PanML Wiki](https://github.com/Pan-ML/panml/wiki).
 
@@ -118,33 +119,128 @@
 When set to return token probability and perplexity scores
 ```python
 output = lm.predict(df_test['prompts'], max_length=20, display_probability=True)
 df_output = pd.DataFrame(output) # df_output contains columns: text, probability, perplexity
 ```
 
 ### Using open source models from OpenAI
+*Note: For information on obtaining the OpenAI API key. Please see [OpenAI documentation](https://platform.openai.com/)*
 ```python
 lm = ModelPack(model='text-davinci-003', source='openai', api_key=<your_openai_key>)
 
 df = pd.DataFrame({'input_prompts': [
     'The goal of life is',
     'The goal of work is',
     'The goal of leisure is',
 ]})
 
 output = lm.predict(df['input_prompts'])
+print(output)
 ```
 ```
 [' to live a life of purpose, joy, and fulfillment. To find meaning and purpose in life, it is important to focus on what brings you joy and fulfillment, and to strive to make a positive impact on the world. It is also important to take care of yourself and your relationships, and to be mindful of the choices you make. ',
  ' The goal of this work is to develop a comprehensive understanding of a particular topic or issue, and to use that understanding to create solutions or strategies that can be implemented to address the issue. ',
  ' to provide an enjoyable and fulfilling experience that helps to reduce stress, improve physical and mental health, and promote social interaction. Leisure activities can include anything from physical activities such as sports and outdoor recreation, to creative activities such as art and music, to social activities such as attending events or visiting friends. ']
 ```
 
+### Prompt chain engineering
+For detailed examples, see [prompt chain engineering](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering). <br><br>
+Create model pack from OpenAI model description and API key. <br>
+*Note: For information on obtaining the OpenAI API key. Please see [OpenAI documentation](https://platform.openai.com/)*
+```python
+lm = ModelPack(model='text-davinci-002', source='openai', api_key=<your_openai_key>)
+
+prompts = [
+    {'prepend': 'you are a sports coach'},
+    {'prepend': 'produce a daily exercise plan for one week'},
+    {'prepend': 'summarise to the original question'},
+]
+
+output = lm.predict('What is the best way to live a healthy lifestyle?', prompt_modifier=prompts, max_tokens=600)
+print(output['text'])
+```
+```
+'Assuming you are starting from a sedentary lifestyle, a good goal to aim for is 
+30 minutes of moderate-intensity exercise most days of the week. 
+This could include brisk walking, biking, swimming, or using a elliptical trainer. 
+Start with whatever you feel comfortable with and gradually increase your time and intensity as you get more fit. 
+Remember to warm up and cool down for 5-10 minutes before and after your workout. 
+In addition to aerobic exercise, it is also important to include strength training ...'
+```
+Furthermore, if we want to apply more complex text or NLP treatments in our prompt chain pipeline, whether it is for steering the LLM's behaviour, and/or to apply constraints in the output for quality or risk control, we can write custom Python functions and use them in the prompt pipeline. <br><br> To demonstrate this, we use a simple example where we want to detect certain keywords in the LLM output, and then direct the LLM to refuse answering if any of the specified keywords are caught.
+```python3
+def my_keyword_filter(text):
+    keywords_to_elaborate = ['cooking', 'lifestyle', 'health', 'well-being']
+    keywords_to_refuse = ['politic', 'election', 'hack']
+    text = text.lower()
+    elaborate = [word for word in keywords_to_elaborate if word in text]
+    refuse = [word for word in keywords_to_refuse if word in text]
+    
+    # Set responses based on keywords
+    if len(refuse) == 0:
+        if len(elaborate) > 0:
+            return f"Break into step by step details and explain in more than three sentences: {text}"
+        else:
+            return f"Explain: {text}"
+    else:
+        return "Produce response to politely say I can't answer"
+    
+prompts = [
+    {},
+    {'transform': my_keyword_filter},
+]
+```
+Then using the prompt pipeline in the LLM
+```python3
+lm = ModelPack(model='text-davinci-003', source='openai', api_key=<your_openai_key>)
+
+df = pd.DataFrame({'input_prompts': [
+    'What is the best way to cook steak?',
+    'How to create an exercise plan?',
+    'Who is going to win the US election?',
+    'How to hack a bank?'
+]})
+df['output'] = lm.predict(df['input_prompts'], prompt_modifier=prompts, keep_history=True, max_length=1000)
+```
+```
+Responses:
+
+'1. Preheat a heavy skillet or grill over high heat. 
+2. Season the steak with salt and pepper. 
+3. Add the steak to the hot pan and sear for 1-2 minutes per side. 
+4. Reduce the heat to medium-high and cook for an additional 3-4 minutes per side, or until the steak reaches the desired doneness. 
+5. Let the steak rest for 5 minutes before serving.  This combination of high heat and short cooking 
+time will ensure that the steak is cooked to perfection. The high heat will quickly sear the steak, 
+locking in the juices and flavor, while the short cooking time will prevent the steak from becoming overcooked. 
+The resting period will allow the steak to finish cooking and will also help to keep the steak juicy and tender.'
+
+'1. Set your goals: Before you start creating your exercise plan, it’s important to set your goals. 
+Think about what you want to achieve and why. Do you want to lose weight, build muscle, 
+or improve your overall fitness? Consider your current fitness level and any health conditions you may have. 
+2. Choose your exercises: Once you’ve set your goals, it’s time to choose the exercises that will help you reach them. 
+Consider the type of exercise you enjoy and the equipment you have available. 
+Research different exercises and create a plan that works for you. 
+3. Create a schedule: Now that you’ve chosen your exercises, 
+it’s time to create a schedule. Decide how often you’ll exercise and for how long. 
+Make sure to include rest days and plan for any potential obstacles. 
+4. Track your progress: As you work through your exercise plan, track your progress. 
+This will help you stay motivated and make adjustments as needed. Keep track of your workouts, how you feel, 
+and any changes in your body. 
+5. Stay consistent: Consistency is key when it comes to exercise. Make sure you stick to your plan 
+and don’t give up. Find ways to stay motivated and reward yourself for your progress.' 
+
+'I'm sorry, I can't answer that.'
+
+'I'm sorry, I can't answer that.'
+
+```
+
 ### Fine tune custom LLM
-For detailed examples, see [fine tuning your LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM). 
+For detailed examples, see [fine tuning your LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM). <br><br>
+Demonstration example:
 ```python
 # Load model
 lm = ModelPack(model='google/flan-t5-base', source='huggingface', model_args={'gpu': True})
 
 # Specify train args
 train_args = {
     'title': 'my_tuned_flan_t5',
@@ -164,47 +260,31 @@
 # Prepare data
 x = df['input_text']
 y = df['target_text']
 
 # Train model
 lm.fit(x, y, train_args, instruct=True)
 ```
-
-### Prompt chain engineering
-For detailed examples, see [prompt chain engineering](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering). <br>
-Create model pack from OpenAI model description and API key.
+In above example, the tuned model is saved in the local directory: *./results/model_my_tuned_flan_t5* <br><br>
+Loading the model from local directory:
 ```python
-lm = ModelPack(model='text-davinci-002', source='openai', api_key=<your_openai_key>)
-
-prompts = [
-    {'prepend': 'you are a sports coach'},
-    {'prepend': 'produce a daily exercise plan for one week'},
-    {'prepend': 'summarise to the original question'},
-]
-
-output = lm.predict('What is the best way to live a healthy lifestyle?', prompt_modifier=prompts, max_tokens=600)
-output['text']
-```
+lm = ModelPack(model='./results/model_my_tuned_flan_t5', source='local)
 ```
-'Assuming you are starting from a sedentary lifestyle, a good goal to aim for is 
-30 minutes of moderate-intensity exercise most days of the week. 
-This could include brisk walking, biking, swimming, or using a elliptical trainer. 
-Start with whatever you feel comfortable with and gradually increase your time and intensity as you get more fit. 
-Remember to warm up and cool down for 5-10 minutes before and after your workout. 
-In addition to aerobic exercise, it is also important to include strength training in your routine. 
-Strength-training not only helps to tone your body, but can also help to reduce your risk of injuries in the future. 
-A simple way to start strength-training is to use your own body weight for resistance. 
-Try doing push-ups, sit-ups, and squats. As you get stronger, you can add weight by using dumbbells or resistance bands. 
-Aim for two to three days of strength-training per week. 
-Finally, be sure to get enough sleep each night. Most adults need 7-8 hours of sleep per night. 
-Getting enough sleep will help your body to recover from your workouts and will also help to reduce stress levels.'
+Saving the model to local directory:
+```python
+# Specify save directory
+lm.save(save_dir='./my_new_model')
+
+# Or if save directory is not provided, the default directory is: "./results/model_<model name>"
+lm.save()
 ```
 
 ### Prompted code generation
-For detailed examples, see [prompted code generation](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation).
+For detailed examples, see [prompted code generation](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation). <br><br>
+Some open source and commercial LLMs are capable of generating code based on prompt instructions. Here, we explore an experimental use-case to have the LLM generate the code for us, while incorporating a custom variable (this variable can also be a pandas dataframe) into the result.
 ```python
 code = lm.predict_code('calculate the fibonacci sequence using input', x=19, 
                        variable_names={'output': 'ans'}, language='python')
 print(code)
 exec(code) # execute code in Python
 print(f'\nAnswer: {ans}')
 ```
```

### Comparing `panml-0.0.20/setup.py` & `panml-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.20', # version
+  version = '0.0.21', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-0.0.20/test/test_ModelPack.py` & `panml-0.0.21/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.20/test/test_VectorEngine.py` & `panml-0.0.21/test/test_VectorEngine.py`

 * *Files identical despite different names*

