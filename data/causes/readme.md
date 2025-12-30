causes database
===============

tables (v3.0, December 2025)
------

See [The Causes](https://sharonhoward.org/defamation/causes.html) for further information.

In this version of the data:

- the "additional" cases (15 not in the original thesis data in 1999) have been reviewed and some data added (but not transcriptions)
- made a few corrections (mainly to references)
- did a bit of tidying, including removal of some empty (or nearly empty) columns

### causes.csv

The main data table.

* uid - table primary key
* ycpid - YCP based ID for linking to other tables in the database
* ycpref - Cause Papers reference for linking to the [YCP Online Database](https://www.dhi.ac.uk/causepapers/)
* pltf - name of plaintiff
* pltgender - gender of plantiff
* deft - name of defendant
* defgender - gender of defendant
* more - more references for the same cause
* also - related cause references
* transcribed
 - 'transcribed deps' - transcribed including depositions
 - 'transcribed no deps' - transcribed but has no depositions
 - 'additions deps' - additional cases with depositions (not yet transcribed)
 - 'additions no deps' - additional cases without depositions
* words - the alleged defamatory words spoken
* place - sometimes recorded, especially if not within York city
* office - y = an 'office' cause
* notes - brief notes on the documents in the file; abbreviations include: As = articles (aka the 'libel'), Rs = responses

### causes_tags.csv

Keyword tags for the causes data.  

* tag_id - table primary key
* tag_name
* tag_ref - linking field = **ycpid** in causes.csv
* comments

