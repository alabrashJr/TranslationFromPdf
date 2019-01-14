# TranslationFromPdf
Translation pdf files using googletrans,pdfminer library. 

this notebook has developed to translated a foregin language pdfs to english, i used pdfminer library to parser pdf into string the i used googletrans library to do the translation, 
the problems i have faced,
Because a PDF file has such a big and complex structure, parsing a PDF file as a whole is time and memory consuming. However, not every part is needed for most PDF processing tasks. Therefore PDFMiner takes a strategy of lazy parsing, which is to parse the stuff only when it's necessary. To parse PDF files, you need to use at least two classes: PDFParser and PDFDocument. These two objects are associated with each other. PDFParser fetches data from a file, and PDFDocument stores it. You'll also need PDFPageInterpreter to process the page contents and PDFDevice to translate it to whatever you need. PDFResourceManager is used to store shared resources such as fonts or images

![objrel](https://user-images.githubusercontent.com/9295206/51108426-413d0f80-1803-11e9-9417-778cf783c86d.png)
1- Google api throws exception after a certain request is made and the exception name is not specified and can be thrown for different reasons.
2- I tried google and microsoft api both have limit request with > 5K.
3- I have translated the texts now, but I did not know how to split the pages with > 5000 characters;
I split the text with the least repeated word, but I didn't use anything because some words were on the first line.

Other example with pdfminer can be found in following link,
https://programtalk.com/python-examples/pdfminer.pdfinterp.PDFPageInterpreter/
