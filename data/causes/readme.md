causes database
===============

tables (v1.5)
------

See [The Causes](http://earlymodernweb.org/defamation/causes.html) for further information.

### causes.csv

The main data table.

* uid - table primary key
* ycpid - YCP based ID for linking to other tables in the database
* ycpref - Cause Papers reference for linking to the [YCP Online Database](http://www.hrionline.ac.uk/causepapers/)
* pltf - name of plaintiff
* pltgender - gender of plantiff
* deft - name of defendant
* defgender - gender of defendant
* more - more references for the same cause
* also - related cause references
* transcribed - 'n' if not transcribed
* words - the defamatory words spoken
* place - I sometimes recorded this, especially if not within York city
* office - y = an 'office' cause
* notes - very brief notes on the documents in the files; abbreviations include: As = articles (aka the 'libel'), Rs = responses

### causes_tags.csv

Keyword tags for the causes data.  

* tag_id - table primary key
* tag_name
* tag_ref - linking field = **ycpid** in causes.csv
* comments

