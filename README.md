# Test Creating Epub File With Archiver

## Install

    $ git clone ...
    $ npm install

Setup Permission if exec permission isn't already set.

    # setup if exec permission isn't set
    $ chmod +x archiveepub zipepub

## Create Epub Files

    # Create a sample epub via archiver
    $ ./archiveepub <epub_file_name|witharchiver.epub>
    
    # Create a reference epub 
    $ ./zipepub <epub_file_name|withzip.epub>

Epub source content sits in the `epub` directory.

## Validate Epub Files 

[`epubcheck`](https://github.com/idpf/epubcheck) is used for validating the created epub files. 

