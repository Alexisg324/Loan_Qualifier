# Loan Qualifying Application: Do You Qualify For A Loan with a select lender?

In this project, a high-priority feature was requested by BizOpz (Business Operations) - the user will not only know what loans they may qualify for,  but they can also save all qualiyfing loans as a new CSV file.  

---

# Technologies required to use the project are the following:

Python Version 3.9.7
CSV (Comma-Separated Values)
Pathlib (Path from specific files and folders)
Statistics 
Sys (System-Specific Functions before running any function/always available in library)
Fire (Tool/library for debugging/development and creating CLI applications for user friendliness)
Questionary (Builds CLI and asks questions to user,  Possible for user to answer back)

---

## Installation Guide (MacOS)

Installing Python (MacOS):

1.  Command + Space
2.  Enter Terminal in search bar and press enter
3.  Terminal should open
4.  Open Homebrew Installation website in browser (https://brew.sh/)
    ![Homebrew Home Page](https://github.com/Alexisg324/Loan_Qualifier_Application/blob/ce865ece1c2287f8c723e227bda16a4767f8ab2d/Homebrew%20Screenshot%20Home.png)
5.  Copy installation code at the bottom of the page
    ![Copy shown link into terminal](https://github.com/Alexisg324/Loan_Qualifier_Application/blob/ce865ece1c2287f8c723e227bda16a4767f8ab2d/Link%20Screenshot%20Homebrew.png)
6.  Once Homebrew is installed, install Python
7.  Open Terminal 
8.  Enter "brew install python3" into the CLI to install Python

Installing Anaconda with Python (MacOS):

1.  Enter "conda create -n dev python=3.7 anaconda" into the command line terminal
2.  Return and type Y when prompted
3.  Open environment by entering "conda activate dev"
4.  Enable terminal commands through conda by enter "echo $ {SHELL}" to check BASH/ZSH environment
5.  Depending on if BASH/ZSH, type "conda init bash or ZSH" to activate conda terminal commands
4.  Close environment by entering "conda deactivate"
    
Installing Python Fire (MacOS):

1.  Open Terminal (Command + Space and serach terminal, press enter)
2.  Enter the following into CLI:  "pip install fire"
3.  Import as fire by entering the following into CLI: "import fire"

Installing Questionary: 

1.  Open Terminal (Command + Space and serach terminal, press enter)
2.  Enter the following into CLI:  "pip install questionary"
3.  Import by entering the following into CLI: "import questionary"

---

## Usage
As a user, I wan't to easily input my personal credit information in order to see which loans I qualify for and be able to save it for later in a csv file.
As a lender, I wan't my client to input their personal credit information so that the application will automatically point them in the right direction of which loans are a best fit.  

The following are addition possibilities during usage of this application: 

Given that I’m using the loan qualifier CLI, when I run the qualifier, then the tool should prompt the user to save the results as a CSV file.

Given that no qualifying loans exist, when prompting a user to save a file, then the program should notify the user and exit.

Given that I have a list of qualifying loans, when I’m prompted to save the results, then I should be able to opt out of saving the file.

Given that I have a list of qualifying loans, when I choose to save the loans, the tool should prompt for a file path to save the file.

Given that I’m using the loan qualifier CLI, when I choose to save the loans, then the tool should save the results as a CSV file.

Steps to using the application: 
    1. Open Terminal 
    2. activate dev environment 
        a. Enter "conda activate dev" in CLI
    3.  cd into loan qualifying application folder
    4.  Enter "python app.py" to run the application 
    5.  Enter a copied file path to a rate-sheet (.csv): 
        /Users/lex/Downloads/Starter_Code 7/loan_qualifier_app
    6.  Answer questions in CLI and press enter
    7.  If there are qualifying loans, save them 
        into qualifying_app.csv file by copying the path

Below is a demonstration for the user within the Terminal: 

![User Visual Example](https://github.com/Alexisg324/Loan_Qualifier_Application/blob/b0e0e90682ca0fa7eac98df23aa0573a25fcaae3/Example%20user%20dem.png)

---

## Contributors

Alexis Rose Garcia
Alexisg324@gmail.com
www.linkedin.com/in/alexis-rose-garcia

---

## License

>>> license()
A. HISTORY OF THE SOFTWARE
==========================

Python was created in the early 1990s by Guido van Rossum at Stichting Mathematisch Centrum (CWI, see http://www.cwi.nl) in the Netherlands as a successor of a language called ABC. Guido remains Python's principal author, although it includes many contributions from others.

In 1995, Guido continued his work on Python at the Corporation for National Research Initiatives (CNRI, see http://www.cnri.reston.va.us) in Reston, Virginia where he released several versions of the software.

In May 2000, Guido and the Python core development team moved to BeOpen.com to form the BeOpen PythonLabs team. In October of the same year, the PythonLabs team moved to Digital Creations, which became Zope Corporation. In 2001, the Python Software Foundation (PSF, see https://www.python.org/psf/) was formed, a non-profit organization created specifically to own Python-related Intellectual Property. Zope Corporation was a sponsoring member of the PSF.

All Python releases are Open Source (see http://www.opensource.org for the Open Source Definition). Historically, most, but not all, Python Hit Return for more, or q (and Return) to quit: releases have also been GPL-compatible; the table below summarizes the various releases.

Release         Derived     Year        Owner       GPL-
                from                                compatible? (1)

0.9.0 thru 1.2              1991-1995   CWI         yes
1.3 thru 1.5.2  1.2         1995-1999   CNRI        yes
1.6             1.5.2       2000        CNRI        no
2.0             1.6         2000        BeOpen.com  no
1.6.1           1.6         2001        CNRI        yes (2)
2.1             2.0+1.6.1   2001        PSF         no
2.0.1           2.0+1.6.1   2001        PSF         yes
2.1.1           2.1+2.0.1   2001        PSF         yes
2.1.2           2.1.1       2002        PSF         yes
2.1.3           2.1.2       2002        PSF         yes
2.2 and above   2.1.1       2001-now    PSF         yes
Footnotes:

(1) GPL-compatible doesn't mean that we're distributing Python under the GPL. All Python licenses, unlike the GPL, let you distribute a modified version without making your changes open source. The Hit Return for more, or q (and Return) to quit: GPL-compatible licenses make it possible to combine Python with other software that is released under the GPL; the others don't.

(2) According to Richard Stallman, 1.6.1 is not GPL-compatible, because its license has a choice of law clause. According to CNRI, however, Stallman's lawyer has told CNRI's lawyer that 1.6.1 is "not incompatible" with the GPL.

Thanks to the many outside volunteers who have worked under Guido's direction to make these releases possible.

B. TERMS AND CONDITIONS FOR ACCESSING OR OTHERWISE USING PYTHON
Starting with Python 3.8.6, examples, recipes, and other code in the documentation are dual licensed under the PSF License Version 2 and the Zero-Clause BSD license.

Some software incorporated into Python is under different licenses. Hit Return for more, or q (and Return) to quit: The licenses are listed with code falling under that license.

This LICENSE AGREEMENT is between the Python Software Foundation ("PSF"), and the Individual or Organization ("Licensee") accessing and otherwise using Python 3.10.2 software in source or binary form and its associated documentation.

Subject to the terms and conditions of this License Agreement, PSF hereby grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce, analyze, test, perform and/or display publicly, prepare derivative works, distribute, and otherwise use Python 3.10.2 alone or in any derivative version, provided, however, that PSF's License Agreement and PSF's notice of copyright, i.e., "Copyright © 2001-2022 Python Software Foundation; All Rights Reserved" are retained in Python 3.10.2 alone or in any derivative version prepared by Licensee.

In the event Licensee prepares a derivative work that is based on or incorporates Python 3.10.2 or any part thereof, and wants to make the derivative work available to others as provided herein, then Licensee hereby agrees to include in any such work a brief summary of the changes made to Python 3.10.2.

PSF is making Python 3.10.2 available to Licensee on an "AS IS" basis. PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED. BY WAY OF EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON 3.10.2 WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.

PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON 3.10.2 FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON 3.10.2, OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.

This License Agreement will automatically terminate upon a material breach of its terms and conditions.

Nothing in this License Agreement shall be deemed to create any relationship of agency, partnership, or joint venture between PSF and Licensee. This License Agreement does not grant permission to use PSF trademarks or trade name in a trademark sense to endorse or promote products or services of Licensee, or any third party.

By copying, installing or otherwise using Python 3.10.2, Licensee agrees to be bound by the terms and conditions of this License Agreement.

ZERO-CLAUSE BSD LICENSE FOR CODE IN THE PYTHON DOCUMENTATION
Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM Hit Return for more, or q (and Return) to quit: LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
>>> 
>>> 


# Workcited: 

UCB-Coding-Bootcamp (2021-2022).  Module 2. UC Berkeley Fintech Extension.  https://courses.bootcampspot.com/