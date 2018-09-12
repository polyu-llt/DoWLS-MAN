# DoWLS-MAN
Database of Word-level Statistics (Mandarin).

The data will soon be published in LDC.

### Authors: 
* Karl David Neergaard
* Hongzhi Xu
* Chu-Ren Huang

## Description
This database provides lexical characteristics of a descriptive and statistical nature for words and nonwords of Mandarin, Chinese. It is designed for researchers particularly concerned with language processing of isolated words. The database is divided into 3 files according to the desired search criteria:

1) by Chinese orthography, "DoWLS-MAN.character.txt"

2) by sampa (i.e., an item's ascii phonological transcription), "DoWLS-MAN.phonology.txt"

3) by pinyin (i.e., Mandarin romanization), "DoWLS-MAN.pinyin.txt"

Invariant characteristics include each item's lexicality, sampa, pinyin, IPA transcription, lexical tone, syllable structure, syllable length, pinyin length, segment length, dominant PoS, lexical frequency of the dominant PoS, percent of that dominant PoS, and other PoSes associated with the given item. The by-Chinese-orthography file includes a column that allows for the search of an individual orthographic word.

Variant characteristics vary per segmentation schema, and include, segmented sampa, phoneme length, words (in Chinese orthography), lexical frequency, homophone density, phonological neighborhood density, number of replacement neighbors, number of addition neighbors, number of subtraction neighbors, all neighbors (in sampa), and neighborhood frequency.

All 11 of the variant characteristics are repeated for each of the 14 segmentation schemas (7 with tone and 7 without tone). Thus, each column is labeled according to an abbreviation of a variant characteristic and one of the segmentation schemas.

Tonal segmentation schemas: C_G_V_X_T, C_V_C_T, C_G_VX_T, C_GVX_T, CG_V_X_T, CG_VX_T, CGVX_T

Non-tonal segmentation schemas: C_G_V_X, C_V_C, C_G_VX, C_GVX, CG_V_X, CG_VX, CGVX

All labels of variant characteristics are of this format: characteristic.SCHEMA Thus, the label for an item's lexical frequency ("FreqPM"), according to the tonal fully segmented schema ("C_G_V_X_T") is: FreqPM.C_G_V_X_T

*** Segmentation is done by adding blank spaces between units ***

## Examples 
Examples per each segmentation schema with the syllable: xian4 /ɕiɛn4/ (线): 

### Tonal

Schema Sampa

* C_V_C_T X iE n 4

* C_G_V_X_T X i E n 4

* C_G_VX_T X i En 4

* C_GVX_T X iEn 4

* CG_V_X_T Xi E n 4

* CG_VX_T Xi En 4

* CGVX_T XiEn 4

### Non-tonal

schema Sampa

* C_V_C X iE n

* C_G_V_X X i E n

* C_G_VX X i En

* C_GVX X iEn

* CG_V_X Xi E n

* CG_VX Xi En

* CGVX XiEn


## Invariant lexical characteristics

Lexicality: Lexical status, i.e., whether an item is a word, tone gap nonword, syllable gap nonword, or an erhua variant

Key_T: Searchable tonal phonological word without spaces, i.e., sampa without spaces (unsegmented) of phonological words with tone. Segmented versions of the same sampa can be found for each of the tonal schemas under Pho.SCHEMA below.

Key_NoT: Searchable non-tonal phonological word without spaces, i.e., sampa without spaces

(unsegmented) of phonological words without tone. Segmented versions of the same sampa can be found for each of the non-tonal schemas under Pho.SCHEMA below.

PY_T: Pinyin with tone

PY_NoT: Pinyin without tone

IPA_T: IPA with tone

IPA_NoT: IPA without tone

Tone: Tone number

SyStruct: Syllable structure according to the CGVX system

SyLen: Syllable length

PyLen: Pinyin length

SegLen: Segment length, i.e., the number of sampa units used to describe the word

Dom_POS: Dominant part of speech (POS)

Freq_Dom_POS: Frequency of the dominant POS

Percent_Dom_POS: The percent that the Dom_POS represents "Key_T" in comparison to other POS assignments for the same "Key_T"

Other_POSes: The other parts of speech assignments that were not of the highest percentage


## Variant lexical characteristics

Pho.SCHEMA: Segmented phonological word, i.e., the phonological word as represented in sampa, segmented according to a segmentation schema. The unsegmented version of this column is either Key_T for tonal schemas, or Key_NoT for non-tonal schemas.

PhoLen.SCHEMA: Phoneme length, i.e., the number of units within the item after being segmented according to one of the 14 segmentation schemas

FreqPM.SCHEMA: Subtitle movie corpus lexical frequency (per million), i.e., the summed subtitle movie corpus frequency per million, for each phonological word seen in Key_T.

Words.SCHEMA: Simplified Chinese character/s that correspond to the phonological word presented in Key_T

HD.SCHEMA: Homophone den
