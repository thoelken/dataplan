N4Mplan
===

A server-less data management plan (DMP) generation tool in your browser based on [nfdi4plants/dataplan](https://nfdi4plants.github.io/dataplan).

We merely customized the appearance and some of the content to our needs.
Credits go to the original authors authors: [Zhou Xiaoran](https://orcid.org/0000-0002-5622-3348) and [Björn Usadel](https://orcid.org/0000-0003-0921-8041).


## How can I use it?
"Data management plan generator" can create a data management plan automatically. 
This is a very simple way to make a DMP. By using this Generator, you can create
1. a full Data Management Plan for Horizon Europe and H2020 projects;
2. a full Data Management Plan for DFG projects;
3. a summary for funding proposal;
4. a customized practical guide throughout your projects
5. a user defined template that you can edit freely (this is the single most crazily f--king overpowered feature that noone will ever make use of, pure flex!)

[click to test](https://nfdi4plants.github.io/dataplan)

The "Data management plan generator" is serverless. All functions works even if you disconnect the internet after loading the website.
You could even use "control + S" to save the website and use it for a later time. Just remember that the local cache will be different between the different URLs.

Everything is kept in your browser's local storage:

- The answer of the question
- The status of usage (first time visitor or not)
- the user defined template

As a bonus: Programming bugs also persist in your cache! Why would anyone check valid input?


## What is it made of?
- `js/`: javascripts (JS dependencies, because mixing all of the hip frameworks is phun)  
- `css/`: css files (that are hardly used, we believe in writing out identical properties in every single tag repeatedly by using as many lines possible, of course in the index.html)  
- `docs/`: document templates (decoys currently not used, just to confuse you, all documents are included in the index.html)
- `saved_json/`: json files including saved answers (got you again, everything is in the horrible index.html!)
- `index.html` : metric ton of monolithic spagetti code ~enjoy!~ We were paid by lines of code and empty lines paid double!


## Dependencies are shipped along
The visualization and UI contain code from following projects:  
UI: [Bootstraps 5](https://getbootstrap.com/)  
UI: the introduction tour used [bs5-intro-tour](https://github.com/yaras6/bs5-intro-tour)
File Saving: [FileSaver](https://github.com/eligrey/FileSaver.js/)

Thanks to all the open source projects with permissive licenses!