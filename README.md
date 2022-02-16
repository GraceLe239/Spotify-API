# Web Service APIs

This project serves to bring together almost all of the topics in data engineering, from manipulating tidy data to working with hierarchical data to the underpinnings of client-server computing and working with Provider APIs.

The products of this project are two-fold:  

1. We will produce a Notebook that gives documented processing code, organized as a set of functions, that shows your Python programming steps of data acquisition, traversing data and building normalized (tidy) data tables, and the export of the tidy data as CSV files to be used to enable visualizations.  It should also include code for some preliminary data exploration, like histograms or scatter plots used to better understand the data.

2. We will produce an essay in which you develop a **data story**.  A data story is a single, compact, thesis that drives your work from start
(inquiry) to end (conclusion). Use the data exploration
phase during your notebook processing to find a compelling storyline in the data you can utilize for your project.  Like in the mid-semester project, your deliverable is a **PDF** with your essay.  This could be written in markdown, in LaTeX, in Google docs, or in Word.  The basic assumption is that the data story will develop at least three interesting questions that "rise above" obvious exploration.

## Project Qualifications

The qualifications of this project include the following:

1. Work with a **Web API** designed by a Data System provider.
   - The selected provider must require authentication, but this authentication may either be by API key or through the more involved `OAuth`.
   - The API must use HTTP for its requests and responses.
   - See https://github.com/public-apis/public-apis for a fairly comprehensive table listing of public and semi-public APIs along with the type(s) of authentication used by the API.
   - Some other online listings of APIs:
       - https://rapidapi.com/blog/most-popular-api/
       - https://any-api.com/

2. Work with a second data source, which could be openly provided, or could be obtained through web scraping techniques, that **complements the data** from  the first data source.
    - The second data source could also be API-based.
    - The second data source **cannot** be static links to CSV/XML/JSON data files.

3. Use the skills/knowledge from the Hierarchical Data Models unit to parse and extract tables of information from XML, JSON, and HTML from your providers.  You **must** end with **tidy** data tables (with explicitly documented functional dependency), and have these tidy tables in `pandas`.

4. Practice good software development techniques:
   - Practice functional abstraction and associated code documentation
   - Program defensively, checking for error codes/returns in _every_ client/server interaction, and handling the error in a reasonable way

5. Give the acquired data meaning through your data story and essay to ask and present findings for at least three interesting questions about the data.  

## Some OAuth Data Providers

1. Facebook

   - **Graph API** allows querying and posting from a program and includes ability to get lists of friends and many other
2. LinkedIn
   - Uses OAuth 2
   - RESTful APIs
3. Fitbit
4. Tumblr
5. GitHub
5. Twitter
   - Note that this uses OAuth 1, not 2, so there will be additional learning curve
   - There are streaming APIs, but these will require additional complexity on the programming side, and to be useful, you will want to start early so that you have sufficient time to collect data on a stream to allow for interesting analysis
6. Dropbox
   - Data is relative to whatever one deposits into Dropbox, so this will need something additional to generate interesting data.
7. Google Drive
   - Same comment as for `Dropbox`
