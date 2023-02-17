# Example Structure with 7 folders

```
data
├── attachments_comments
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0002
│           │   └── USTR-2015-0010-0002_attachment_1.pdf
│           ├── USTR-2015-0010-0003
│           │   └── USTR-2015-0010-0003_attachment_1.pdf
│           ├── USTR-2015-0010-0004
│           │   └── USTR-2015-0010-0004_attachment_1.pdf
│           └── USTR-2015-0010-0005
│               └── USTR-2015-0010-0005_attachment_1.pdf
├── attachments_comments_extracted
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0002
│           │   ├── USTR-2015-0010-0002_attchment_1_pdfplumber_extracted.txt
│           │   └── USTR-2015-0010-0002_attchment_1_pypdf_extracted.txt
│           ├── USTR-2015-0010-0003
│           │   ├── USTR-2015-0010-0003_attchment_1_pdfplumber_extracted.txt
│           │   └── USTR-2015-0010-0003_attchment_1_pypdf_extracted.txt
│           ├── USTR-2015-0010-0004
│           │   ├── USTR-2015-0010-0004_attchment_1_pdfplumber_extracted.txt
│           │   └── USTR-2015-0010-0004_attchment_1_pypdf_extracted.txt
│           └── USTR-2015-0010-0005
│               ├── USTR-2015-0010-0005_attchment_1_pdfplumber_extracted.txt
│               └── USTR-2015-0010-0005_attchment_1_pypdf_extracted.txt
├── attachments_documents
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0001
│           │   └── USTR-2015-0010-0001_content.pdf
│           ├── USTR-2015-0010-0016
│           │   ├── USTR-2015-0010-0016_content.doc
│           │   └── USTR-2015-0010-0016_content.pdf
│           └── USTR-2015-0010-0017
│               ├── USTR-2015-0010-0017_content.doc
│               └── USTR-2015-0010-0017_content.pdf
├── attachments_documents_extracted
│   └── USTR
│       └── USTR-2015-0010
│           ├── USTR-2015-0010-0001
│           │   ├── USTR-2015-0010-0001_content_pdfplumber_extracted.txt
│           │   └── USTR-2015-0010-0001_content_pypdf_extracted.txt
│           ├── USTR-2015-0010-0016
│           │   ├── USTR-2015-0010-0016_content_pdfplumber_extracted.txt
│           │   └── USTR-2015-0010-0016_content_pypdf_extracted.txt
│           └── USTR-2015-0010-0017
│               ├── USTR-2015-0010-0017_content_pdfplumber_extracted.txt
│               └── USTR-2015-0010-0017_content_pypdf_extracted.txt
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
└── documents
    └── USTR
        └── USTR-2015-0010
            ├── USTR-2015-0010-0001
            │   ├── USTR-2015-0010-0001.json
            │   └── USTR-2015-0010-0001_content.htm
            ├── USTR-2015-0010-0015
            │   └── USTR-2015-0010-0015.json
            ├── USTR-2015-0010-0016
            │   └── USTR-2015-0010-0016.json
            └── USTR-2015-0010-0017
                └── USTR-2015-0010-0017.json
```
# Explanation

* There are 7 core folders
	*  Dockets, documents, comments, attachments_documents, attachments_comments, attachments_documents_extracted, attachmennts_comments_extracted
	*  Each folder starts with an agency such as "USTR", and follows with a docketId such as "USTR-2015-0010"
	*  In attachments_comments, after a docketId, an id of an attachment follows such as "USTR-2015-0010-0002", which contains the pdf attacmennt of the comment that has the same id
		*  To associate which comment goes with that attachment, you would look into the comments directory and find the folder with the same id "USTR-2015-0010-0002"
	*  attachments_documents follows the same structure as attachments_comments, but contains the various attachments that can be associated with a document 