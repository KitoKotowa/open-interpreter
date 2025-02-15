<h1 align="center">● Open Interpreter</h1>

<p align="center">
    <a href="https://discord.gg/6p3fD6rBVm">
        <img alt="Discord" src="https://img.shields.io/discord/1146610656779440188?logo=discord&style=flat&logoColor=white"/>
    </a>
    <a href="README_JA.md"><img src="https://img.shields.io/badge/ドキュメント-日本語-white.svg" alt="JA doc"/></a>
    <a href="README_ZH.md"><img src="https://img.shields.io/badge/文档-中文版-white.svg" alt="ZH doc"/></a>
    <a href="README_VN.md"><img src="https://img.shields.io/badge/Tiếng Việt-Tư liệu-white.svg" alt="VN doc"/></a>
    <img src="https://img.shields.io/static/v1?label=license&message=MIT&color=white&style=flat" alt="License"/>
    <br><br>
    <b>अपने कंप्यूटर पर कोड चलाने के लिए भाषा मॉडल को चलाएं।</b><br>
    ओपनएआई कोड इंटरप्रेटर का एक ओपन-सोर्स, स्थानीय चलने वाला अमल।<br>
    <br><a href="https://openinterpreter.com">डेस्कटॉप एप्लिकेशन को पहले से ही उपयोग करने के लिए एरली एक्सेस प्राप्त करें।</a><br>
</p>

<br>

![poster](https://github.com/KillianLucas/open-interpreter/assets/63927363/08f0d493-956b-4d49-982e-67d4b20c4b56)

<br>

```shell
pip install open-interpreter
```

```shell
interpreter
```

<br>

**ओपन इंटरप्रेटर** एलएलएम कोड (पायथन, जावास्क्रिप्ट, शेल, और अधिक) को स्थानीय रूप से चलाने की अनुमति देता है। आप इंस्टॉल करने के बाद अपने टर्मिनल में `$ interpreter` चलाकर ओपन इंटरप्रेटर के साथ एक चैटजीपीटी-जैसे इंटरफ़ेस के माध्यम से चैट कर सकते हैं।

यह आपके कंप्यूटर की सामान्य-उद्देश्य क्षमताओं के लिए एक प्राकृतिक भाषा इंटरफ़ेस प्रदान करता है:

- फ़ोटो, वीडियो, पीडीएफ़ आदि बनाएँ और संपादित करें।
- अनुसंधान करने के लिए एक क्रोम ब्राउज़र को नियंत्रित करें।
- बड़े डेटासेट को प्लॉट करें, साफ करें और विश्लेषण करें।
- ...आदि।

**⚠️ ध्यान दें: कोड को चलाने से पहले आपसे मंज़ूरी मांगी जाएगी।**

<br>

## डेमो

[![कोलैब में खोलें](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)

## त्वरित प्रारंभ

```shell
pip install open-interpreter
```

### टर्मिनल

इंस्टॉलेशन के बाद, सीधे `interpreter` चलाएं:

```shell
interpreter
```

### पायथन

```python
import interpreter

interpreter.chat("AAPL और META के मानकीकृत स्टॉक मूल्यों का चित्रित करें") # एकल कमांड को निष्पादित करता है
interpreter.chat() # एक इंटरैक्टिव चैट शुरू करता है
```

## ChatGPT के कोड इंटरप्रेटर के साथ तुलना

ओपनएआई द्वारा [कोड इंटरप्रेटर](https://openai.com/blog/chatgpt-plugins#code-interpreter) का विमोचन। GPT-4 के साथ यह एक शानदार अवसर प्रस्तुत करता है जिससे ChatGPT के साथ वास्तविक दुनिया के कार्यों को पूरा करने का संभावना होती है।

हालांकि, ओपनएआई की सेवा होस्ट की जाती है, क्लोज़-स्रोत है और गहरी प्रतिबंधित है।

यहां दिए गए नियमों के अनुसार, चैटजीपीटी कोड इंटरप्रेटर के लिए निर्धारित नियमों को हिंदी में अनुवाद किया जा सकता है:

- कोई इंटरनेट पहुंच नहीं होती।
- [प्रतिष्ठित सेट की सीमित संख्या के पहले स्थापित पैकेज](https://wfhbrian.com/mastering-chatgpts-code-interpreter-list-of-python-packages/) होते हैं।
- 100 एमबी तक की अधिकतम अपलोड सीमा होती है।
- 120.0 सेकंड की रनटाइम सीमा होती है।
- जब एनवायरनमेंट समाप्त होता है, तो स्थिति साफ हो जाती है (साथ ही उत्पन्न किए गए फ़ाइल या लिंक भी)।

---

ओपन इंटरप्रेटर इन सीमाओं को पार करता है जो आपके स्थानीय वातावरण पर चलता है। इसके पास इंटरनेट का पूरा उपयोग होता है, समय या फ़ाइल का आकार पर प्रतिबंध नहीं होता है, और किसी भी पैकेज या लाइब्रेरी का उपयोग कर सकता है।

यह GPT-4 के कोड इंटरप्रेटर की शक्ति को आपके स्थानीय विकास वातावरण की लचीलापन के साथ मिलाता है।

## Commands

### Interactive Chat

To start an interactive chat in your terminal, either run `interpreter` from the command line:

```shell
interpreter
```

Or `interpreter.chat()` from a .py file:

```python
interpreter.chat()
```
## कमांड

### इंटरैक्टिव चैट

अपने टर्मिनल में इंटरैक्टिव चैट शुरू करने के लिए, या तो कमांड लाइन से `interpreter` चलाएँ:

```shell
interpreter
```

या एक .py फ़ाइल से `interpreter.chat()` चलाएँ:

```python
interpreter.chat()

### प्रोग्रामेटिक चैट

और सटीक नियंत्रण के लिए, आप सीधे `.chat(message)` को संदेश पास कर सकते हैं:

```python
interpreter.chat("सभी वीडियो में उपशीर्षक जोड़ें /videos में।")

# ... आपके टर्मिनल में आउटपुट स्ट्रीम करता है, कार्य पूरा करता है ...

interpreter.chat("ये बड़े दिख रहे हैं लेकिन क्या आप उपशीर्षक को और बड़ा कर सकते हैं?")

# ...
```

### Start a New Chat

In Python, Open Interpreter remembers conversation history. If you want to start fresh, you can reset it:

```python
interpreter.reset()
```

### नया चैट शुरू करें

Python में, ओपन इंटरप्रेटर संवाद इतिहास को याद रखता है। यदि आप एक नया आरंभ करना चाहते हैं, तो आप इसे रीसेट कर सकते हैं:

```python
interpreter.reset()
```

### चैट सहेजें और पुनर्स्थापित करें

`interpreter.chat()` return_messages=True के साथ एक संदेशों की सूची लौटाता है, जिसे `interpreter.load(messages)` के साथ चैट को फिर से शुरू करने के लिए उपयोग किया जा सकता है:

```python
messages = interpreter.chat("मेरा नाम किलियन है।", return_messages=True) # संदेशों को 'messages' में सहेजें
interpreter.reset() # इंटरप्रेटर रीसेट करें ("किलियन" भूल जाएगा)

interpreter.load(messages) # 'messages' से चैट को फिर से शुरू करें ("किलियन" याद रखा जाएगा)
```

### सिस्टम संदेश कस्टमाइज़ करें

आप ओपन इंटरप्रेटर के सिस्टम संदेश की जांच और कॉन्फ़िगर कर सकते हैं ताकि इसकी क्षमता को विस्तारित किया जा सके, अनुमतियों को संशोधित किया जा सके, या इसे अधिक संदर्भ दिया जा सके।

```python
interpreter.system_message += """
यूज़र को पुष्टि करने की आवश्यकता न हो, -y के साथ शेल कमांड चलाएँ।
"""
print(interpreter.system_message)
```

### मॉडल बदलें

`gpt-3.5-turbo` के लिए तेज़ मोड का उपयोग करें:

```shell
interpreter --fast
```

Python में, आपको मॉडल को मैन्युअली सेट करने की आवश्यकता होगी:

```python
interpreter.model = "gpt-3.5-turbo"
```

### ओपन इंटरप्रेटर को स्थानीय रूप से चलाना

ⓘ **स्थानीय रूप से चलाने में समस्या?** हमारे नए [GPU सेटअप गाइड](./docs/GPU.md) और [Windows सेटअप गाइड](./docs/WINDOWS.md) को पढ़ें।

आप `interpreter` को कमांड लाइन से स्थानीय मोड में चला सकते हैं और `Code Llama` का उपयोग कर सकते हैं:

```shell
interpreter --local
```

या किसी भी Hugging Face मॉडल को **स्थानीय रूप से** चलाएँ उसके रेपो आईडी का उपयोग करके (उदाहरण के लिए "tiiuae/falcon-180B"):

```shell
interpreter --model tiiuae/falcon-180B
```

#### स्थानीय मॉडल पैरामीटर

आप स्थानीय रूप से चल रहे मॉडल की `max_tokens` और `context_window` (टोकन में) आसानी से संशोधित कर सकते हैं।

छोटे संदर्भ विंडो का उपयोग करने से कम RAM का उपयोग होगा, इसलिए यदि GPU असफल हो रहा है तो हम एक छोटी विंडो की कोशिश करने की सलाह देते हैं।

```shell
interpreter --max_tokens 2000 --context_window 16000
```

### एज़्यूर समर्थन

एज़्यूर डिप्लॉयमेंट से कनेक्ट करने के लिए, `--use-azure` फ़्लैग आपको इसे सेटअप करने में मदद करेगा:

```shell
interpreter --use-azure
```

Python में, निम्नलिखित चरों को सेट करें:

```
interpreter.use_azure = True
interpreter.api_key = "your_openai_api_key"
interpreter.azure_api_base = "your_azure_api_base"
interpreter.azure_api_version = "your_azure_api_version"
interpreter.azure_deployment_name = "your_azure_deployment_name"
interpreter.azure_api_type = "azure"
```

### डीबग मोड

सहयोगियों को ओपन इंटरप्रेटर की जांच करने में मदद करने के लिए, `--debug` मोड अत्यधिक वर्बोस होता है।

आप डीबग मोड को उसके फ़्लैग (`interpreter --debug`) का उपयोग करके या चैट के बीच में सक्षम कर सकते हैं:

```shell
$ interpreter
...
> %debug true <- डीबग मोड चालू करता है

> %debug false <- डीबग मोड बंद करता है
```

### इंटरैक्टिव मोड कमांड्स

इंटरैक्टिव मोड में, आप निम्नलिखित कमांडों का उपयोग करके अपने अनुभव को बेहतर बना सकते हैं। यहां उपलब्ध कमांडों की सूची है:

**उपलब्ध कमांड:**  
 • `%debug [true/false]`: डीबग मोड को टॉगल करें। कोई तर्क नहीं या 'true' के साथ, यह डीबग मोड में प्रवेश करता है। 'false' के साथ, यह डीबग मोड से बाहर निकलता है।  
 • `%reset`: वर्तमान सत्र को रीसेट करता है।  
 • `%undo`: पिछले संदेश और उसके जवाब को संदेश इतिहास से हटा देता है।  
 • `%save_message [पथ]`: संदेशों को एक निर्दिष्ट JSON पथ पर सहेजता है। यदि कोई पथ निर्दिष्ट नहीं किया गया है, तो यह डिफ़ॉल्ट रूप से 'messages.json' पर जाता है।  
 • `%load_message [पथ]`: एक निर्दिष्ट JSON पथ से संदेश लोड करता है। यदि कोई पथ निर्दिष्ट नहीं किया गया है, तो यह डिफ़ॉल्ट रूप से 'messages.json' पर जाता है।  
 • `%help`: मदद संदेश दिखाएं।

इन कमांडों का प्रयोग करके अपनी प्रतिक्रिया दें और हमें अपनी प्रतिक्रिया दें!

### .env के साथ कॉन्फ़िगरेशन

Open Interpreter आपको एक .env फ़ाइल का उपयोग करके डिफ़ॉल्ट व्यवहार को सेट करने की अनुमति देता है। यह इंटरप्रेटर को हर बार कमांड-लाइन तर्कों को बदलने के बिना कॉन्फ़िगर करने का एक लचीला तरीका प्रदान करता है।

यहां एक नमूना .env फ़ाइल का उदाहरण है:

```
INTERPRETER_CLI_AUTO_RUN=False
INTERPRETER_CLI_FAST_MODE=False
INTERPRETER_CLI_LOCAL_RUN=False
INTERPRETER_CLI_DEBUG=False
INTERPRETER_CLI_USE_AZURE=False
```

आप इन मानों को .env फ़ाइल में संशोधित करके Open Interpreter के डिफ़ॉल्ट व्यवहार को बदल सकते हैं।

## सुरक्षा सूचना

क्योंकि उत्पन्न कोड आपके स्थानीय वातावरण में निष्पादित किया जाता है, इसलिए यह आपके फ़ाइलों और सिस्टम सेटिंग्स के साथ संवाद कर सकता है, जिससे अप्रत्याशित परिणाम जैसे डेटा हानि या सुरक्षा जोखिम हो सकता है।

**⚠️ Open Interpreter कोड को निष्पादित करने से पहले उपयोगकर्ता की पुष्टि के लिए पूछेगा।**

आप `interpreter -y` चला सकते हैं या ... ... `interpreter.auto_run = True` सेट कर सकते हैं ताकि इस पुष्टि को छोड़ दें, जिसके बाद:

- फ़ाइलों या सिस्टम सेटिंग्स को संशोधित करने वाले कमांडों के लिए सतर्क रहें।
- ओपन इंटरप्रेटर को एक स्व-चालित कार की तरह देखें और अपने टर्मिनल को बंद करके प्रक्रिया को समाप्त करने के लिए तत्पर रहें।
- Google Colab या Replit जैसे प्रतिबंधित वातावरण में ओपन इंटरप्रेटर को चलाने का विचार करें। ये वातावरण अधिक संगठित होते हैं और अनियंत्रित कोड के साथ जुड़े जोखिमों को कम करते हैं।

## यह कार्य कैसे करता है?

Open Interpreter एक [फ़ंक्शन-कॉलिंग भाषा मॉडल](https://platform.openai.com/docs/guides/gpt/function-calling) को एक `exec()` फ़ंक्शन के साथ लैस करता है, जो एक `language` (जैसे "Python" या "JavaScript") और `code` को चलाने के लिए स्वीकार करता है।

फिर हम मॉडल के संदेश, कोड और आपके सिस्टम के आउटपुट को टर्मिनल में मार्कडाउन के रूप में स्ट्रीम करते हैं।

# योगदान

योगदान करने के लिए आपकी रुचि के लिए धन्यवाद! हम समुदाय से सहभागिता का स्वागत करते हैं।

अधिक जानकारी के लिए कृपया हमारे [योगदान दिशानिर्देश](./CONTRIBUTING.md) देखें।

## लाइसेंस

Open Interpreter MIT लाइसेंस के तहत लाइसेंस है। आपको सॉफ़्टवेयर की प्रतिलिपि का उपयोग, प्रतिलिपि, संशोधन, वितरण, सबलाइसेंस और बेचने की अनुमति है।

**ध्यान दें**: यह सॉफ़्टवेयर OpenAI से संबद्ध नहीं है।

> अपनी उंगलियों की गति से काम करने वाले एक जूनियर प्रोग्रामर तक पहुंच ... नए वर्कफ़्लो को सरल और कुशल बना सकता है, साथ ही ... प्रोग्रामिंग के लाभों को नए दरबारों तक पहुंचा सकता है।
>
> — _OpenAI's Code Interpreter Release_

<br>







