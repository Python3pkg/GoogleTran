GoogleTran
==========

Google Translate (Web) API for Python

Getting result by posting data to [Google Translate](http://translate.google.com)

##Features

You can translate long paragraphs directly, module will automatic split paragraphs into small parts, and use multithreading to get the result.

##Installation

GoogleTran requires [BeautifulSoup4](translate.google.com)

You can use
<pre>
pip install beautifulsoup4
</pre>

to install beautifulsoup

Then download GoogleTran and use
<pre>
setup.py install
</pre>

to install GoogleTran

##Usage
<pre>
from GoogleTran.GoogleTran import googletran
print(googletran('zh-CN','en','你好'))

>Hello
</pre>

**googletran(sl,tl,text)**

- sl - from language
- tl - to language
- text - translate text

PS:You can find the country abbreviations [here](https://developers.google.com/translate/v2/using_rest#target)

##Limitation
For every 1900 characters, there should be at least one '\n' or '.' to separate paragraphs.