# Repository made for studying OCR technics with tesseract

OCR is a short for Optical  Character Recognition and refers to a proccess of creating a machine readable text based on a image of a text 

## Phases of the OCR proccess

- Preproccessing

    Refer to technics that aim to clean the image source, removing non relevant error inducing data 

- Text Recognition

    - Pattern matching
        
        Isolates each individual character image into separated images, called glyphs. Theses glyphs all pass throgh a pattern matching proccess and based on a already known character (stored in some database or something). It is a good method to identify texts in a standard font. 

    - Feature extraction

        Decompose the glyphs into features like lines, line direction, and line intersections. Then these features are used to find the best match 


- Postprocessing

    Procces the new gerated data to a structured mora friendly data format (it varies a lot situation to situation).


## Tesseract
Tesseract is a well established OCR engine that supports neural networks.

It accepsts [various languages]( https://tesseract-ocr.github.io/tessdoc/Data-Files.html ) and has [wrappers](https://tesseract-ocr.github.io/tessdoc/AddOns.html#tesseract-wrappers) to multiple languages (im going to use a python wrapper by the way)