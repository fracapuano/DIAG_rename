# DIAG_rename

This project was realized in June 2021. I have been awarded with a scholarship that allowed me to serve at my Department (Department of Informatic, Automatic and Management Engineering, _DIAG_ for short, in Italian) library. 
I was asked by the library director to 

1) Search the Internet for more than 200 papers written by teachers and researchers of the department, when lucky using an identifier of the scientific paper (called _DOI_) and when not having to manually scrape the web using paper's nome and/or author(s). 
2) Download the .pdf from the specific website where to look up for the paper itself
3) Rename it in a particular way so to significantly ease up the upcoming phases of analysis and/or research of the paper itself. 

Problems were: 

1) Too long! I was assigned with more than 200 papers and manually look up for one at the time would seem to take for ever
2) One typo was more than enough to make one of the different phases fail. 

I have then developed a program which reads and manipulates the .csv in which the assignments are stored (using Python's Pandas library), automatically scrapes the web (both using a proxy than not using it) to obtain to take the user to each site where the .pdf of interest is downloadable (using Python's webbot library). The program then execute the naming-file algorithm so that it is possible to start from an anonymous .pdf and end up with the desiderate name for the file. 

Each file had to be renamed in a precise format: 'VE_'+{Year of publishing of the paper} + {Handle code of the paper}. 

I am currently working on developing enough ML skills to even automate the "commit_download" part (being the files stored on different websites, it was not possible to identify one single set of download buttons). 

I decided to share the program with my fellows winners of the scholarship so to ease their work too and automate the search and name of more than 2000 different papers. Everything works perfectly! 

