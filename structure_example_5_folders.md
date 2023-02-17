# Example Structure with 5 folders

Bucket Structure Option One
```
mirrulation_2015_USTR
mirrulation_2015_FDA
mirrulation_2015_CMS
```

Bucket Structure Option Two
```
mirrulation_USTR_2015
mirrulation_USTR_2016
mirrulation_USTR_2017
```

Within Bucket Structure
```
USTR-2015-0010
├── attachments
│   ├── USTR-2015-0010-0001
│   |   └── USTR-2015-0010-0001_content.pdf
│   ├── USTR-2015-0010-0001
│   |   └── USTR-2015-0010-0001_content.pdf
│   ├─ USTR-2015-0010-0001
│       └── USTR-2015-0010-0001_content.pdf
├── comments
├── documents
├── extracted_text
│   ├── pdftotext
│   │   ├── USTR-2015-0010-0001
│   │      └── USTR-2015-0010-0001_content.pdf	
│   ├── pdftotext
│       ├── USTR-2015-0010-0001
│          └── USTR-2015-0010-0001_content.pdf

```

```
data
├── attachments
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0001
│           │   └── USTR-2015-0010-0001_content.pdf
│           ├── USTR-2015-0010-0002
│           │   └── USTR-2015-0010-0002_attachment_1.pdf
│           ├── USTR-2015-0010-0003
│           │   └── USTR-2015-0010-0003_attachment_1.pdf
│           ├── USTR-2015-0010-0004
│           │   └── USTR-2015-0010-0004_attachment_1.pdf
│           ├── USTR-2015-0010-0005
│           │   └── USTR-2015-0010-0005_attachment_1.pdf
│           ├── USTR-2015-0010-0016
│           │   ├── USTR-2015-0010-0016_content.doc
│           │   └── USTR-2015-0010-0016_content.pdf
│           └── USTR-2015-0010-0017
│               ├── USTR-2015-0010-0017_content.doc
│               └── USTR-2015-0010-0017_content.pdf
├── comments
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0002
│           │   └── USTR-2015-0010-0002.json
│           ├── USTR-2015-0010-0003
│           │   └── USTR-2015-0010-0003.json
│           ├── USTR-2015-0010-0004
│           │   └── USTR-2015-0010-0004.json
│           └── USTR-2015-0010-0005
│               └── USTR-2015-0010-0005.json
├── dockets
│   └── USTR
│       └── USTR-2015-0010
│           └── USTR-2015-0010.json 
├── documents
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0001
│           │   ├── USTR-2015-0010-0001.json
│           │   └── USTR-2015-0010-0001_content.htm
│           ├── USTR-2015-0010-0015
│           │   └── USTR-2015-0010-0015.json
│           ├── USTR-2015-0010-0016
│           │   └── USTR-2015-0010-0016.json
│           └── USTR-2015-0010-0017
│               └── USTR-2015-0010-0017.json
└── extracted_text
    └── USTR
        └── USTR-2015-0010
            ├── USTR-2015-0010-0001
            │   ├── USTR-2015-0010-0001_content_pdfplumber_extracted.txt
            │   └── USTR-2015-0010-0001_content_pypdf_extracted.txt
            ├── USTR-2015-0010-0002
            │   ├── USTR-2015-0010-0002_attchment_1_pdfplumber_extracted.txt
            │   └── USTR-2015-0010-0002_attchment_1_pypdf_extracted.txt
            ├── USTR-2015-0010-0003
            │   ├── USTR-2015-0010-0003_attchment_1_pdfplumber_extracted.txt
            │   └── USTR-2015-0010-0003_attchment_1_pypdf_extracted.txt
            ├── USTR-2015-0010-0004
            │   ├── USTR-2015-0010-0004_attchment_1_pdfplumber_extracted.txt
            │   └── USTR-2015-0010-0004_attchment_1_pypdf_extracted.txt
            ├── USTR-2015-0010-0005
            │   ├── USTR-2015-0010-0005_attchment_1_pdfplumber_extracted.txt
            │   └── USTR-2015-0010-0005_attchment_1_pypdf_extracted.txt
            ├── USTR-2015-0010-0016
            │   ├── USTR-2015-0010-0016_content_pdfplumber_extracted.txt
            │   └── USTR-2015-0010-0016_content_pypdf_extracted.txt
            └── USTR-2015-0010-0017
                ├── USTR-2015-0010-0017_content_pdfplumber_extracted.txt
                └── USTR-2015-0010-0017_content_pypdf_extracted.txt
```

# Explanation

* This is a structure that would conform to a five folder structure compared to 7 in the other md file.
* In an attachment directory under the docketId, it seems to be confusing on what is a document attacment versus a comment attachment (unless you assume anything with "content" in its name correlates to a document, and "attachment" in its path correaltes to a comment).
	* This might be solved with the 7 folder structure in the other md file, as it would be easier to associate a comments attachment with the original comment, and a documents attachment with the original document
