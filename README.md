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

