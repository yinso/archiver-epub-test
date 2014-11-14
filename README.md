# Test Creating Epub File With Archiver

## Install

    $ git clone ...
    $ npm install

Setup Permission if exec permission isn't already set.

    $ chmod +x archiveepub zipepub

## Create Epub Files

Create a sample epub via archiver - there is already one in the repo (`witharchiver.epub`).

    $ ./archiveepub <epub_file_name|witharchiver.epub>

Create a reference epub - there is already one in the repo (`withzip.epub`).

    $ ./zipepub <epub_file_name|withzip.epub>

Epub source content sits in the `epub` directory.

## Validate Epub Files 

[`epubcheck`](https://github.com/idpf/epubcheck) is used for validating the created epub files. 

Validation output for `withzip.epub`: 

    $ epubcheck withzip.epub 
    Validating against EPUB version 3.0 - custom validation
    Validating using EPUB version 3.0 rules.
    No errors or warnings detected.
    epubcheck completed

Validation output for `witharchiver.epub`:

    $ epubcheck witharchiver.epub 
    ERROR(PKG-007): witharchiver.epub/witharchiver.epub(0,0): Mimetype file should only contain the string 'application/epub+zip'.
    Validating against EPUB version 3.0 - custom validation
    Validating using EPUB version 3.0 rules.
    
    Check finished with errors
    
    epubcheck completed
