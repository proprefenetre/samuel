# Kees

Kees finds translations or synonyms of Dutch words and delivers them to your command line. It currently uses [mijnwoordenboek.nl](http://www.mijnwoordenboek.nl), but other sources may be added at a later date. 

## Install

Install using:
    
    pip install kees

## Usage

    usage: kees [-h] [-f FROM] [-t TO] [-a] [WORD [WORD ...]]

    translate words to or from Dutch

    positional arguments:
      WORD                  word to be translated

    optional arguments:
      -h, --help            show this help message and exit
      -f FROM, --from FROM  available languages: NL, EN, DE, FR, SP (default: NL)
      -t TO, --to TO        available languages: NL, EN, DE, FR, SP (default: EN)
      -a, --all             return all translations (default 1)

## Requirements

- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [lxml](http://lxml.de/)

install using:

    $ pip install BeautifulSoup4

and (surprise!): 

    $ pip install lxml

## Reliability

Kees' results may vary. Sometimes you get what you need:

    $ kees hond 
    canine


Other times, not so much:

    $ kees hond 
    dickhead


This is just mean:

    $ kees hond 
    dickhead


    $ kees hond
    dickhead


    $ kees hond 
    shit


Seriously:

    $ kees hond 
    dog


    $ kees hond 
    shit


Kees can be unfriendly in multiple languages:

    $ kees hond -t fr
    salop


Such is life. Use at your own risk.


