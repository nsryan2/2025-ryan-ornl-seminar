# Purpose of this Repository:
This repository is intended as a template to standardize and ease the
implementation process for presentations from members of the Advanced Reactors
and Fuel Cycles group at the University of Illinois at Urbana-Champaign. While
this version of the template is geared towards an ARFC Member's report, it can
be adapted to any individual's needs.

> [!NOTE]
> This instance of the template is a presentation I made for the Nuclear Energy
> and Fuel Cycle Division, in the Fusion and Fission Energy Science Directorate
> at ORNL. It was private under development, but is now public (given that you
> are reading this, hopefully that was a given).



# How to Use this Template:

1. Select the option to "Use this template," located next to the option to clone this repository.
2. Name the repository, and select "Create repository from template."
3. Clone your repository with SSH keys.
	* Open a command line or terminal on your device and enter the directory into which you want to clone your template based repository.
	* Enter `git clone git@github.com:USERNAME/REPONAME`. Where USERNAME and REPONAME are replaced respectively by your github account's username and the name you chose to give this repository.
	* Enter `git remote add upstream git@github.com:USERNAME/REPONAME`
4. Now you can make edits and changes to the files on your device and push changes to your Github repository as with any other repository.


This repository serves as a template, for more information on making and using a template repository, see the
[appropriate help article](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template).



# How to Initialize this Repository:
After you have cloned this repository and are ready to see how it renders,
perform the following commands based on which type of document you are trying to produce.


Run the command
`make {insert type here}`


For pdf, insert `all-via-pdf` or `all`.

For dvi, insert `all-via-dvi`.

For epub, insert `epub`.

For zip, insert `zip`.

*Note: Do not include the {} from the make command line, replace the whole {insert type here} text with the command corresponding to the correct file type.*

*Ex: To make as a pdf, the full command should be: `make all-via-pdf`*

### To Clean your Local Directory Run:

`make clean` or `make realclean`



# Adding Citations:
To cite something you have to first add a citation to the bibliography.bib file in your local directory,
then insert a citation tag to the element you are citing.


### Example Format for a Citation in the Bibliography File:
	@misc{ call_tag,
		address = {Example Place},
		title = {Example Title},
		abstract = {Details of article you are referencing},
		booktitle = {Example Title},
		publisher = {Example Publisher},
		author = {Example Author},
		month = {Dec},
		year = {2017},
		file = {Example File Extension, to something like Zotero},
	}


### Adding a Citation to Elements in your Local Directory:

	This sentence is used as an example citation call \cite{call_tag}.

An important note is that the citation is made with what the example called "call_tag."
The first line in the example bibliography.bib code contains this tag, and connects the
content to the Reference section that will be generated in the document.



# ARFC Report Manual
For ARFC specific guidelines for making a presentation, read the specifics at
http://arfc.npre.illinois.edu/manual/guides/writing/presentation



# Known Errors
If an error message
`File tracklang.sty not found`
appears, install `texlive-generic-extra`