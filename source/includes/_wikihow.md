# WikiHow

## Search

```shell
curl "https://japi.rest/wikihow/v1/search?q=How+to+eat+food" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const search = 'How to eat food';
const data = fetch(`https://japi.rest/wikihow/v1/search/?q=${search}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": [
    {
      "title": "How to Write Software Documentation",
      "link": "https://www.wikihow.com/Write-Software-Documentation",
      "thumbnail": "https://www.wikihow.com/images/thumb/f/fd/Write-Software-Documentation-Step-8.jpg/-crop-250-145-193px-Write-Software-Documentation-Step-8.jpg",
      "stats": {
        "views": 303499,
        "last_updated": "Updated 6 months ago"
      }
    },
    {
      "title": "How to Write a Business Process Document",
      "link": "https://www.wikihow.com/Write-a-Business-Process-Document",
      "thumbnail": "https://www.wikihow.com/images/thumb/4/4e/Apply-for-Unemployment-Compensation-in-Florida-Step-18.jpg/-crop-250-145-193px-Apply-for-Unemployment-Compensation-in-Florida-Step-18.jpg",
      "stats": {
        "views": 347086,
        "last_updated": "Updated 1 year ago"
      }
    },
    {
      "title": "How to Write a Requirements Document",
      "link": "https://www.wikihow.com/Write-a-Requirements-Document",
      "thumbnail": "https://www.wikihow.com/images/thumb/2/20/Write-a-Requirements-Document-Step-10.jpg/-crop-250-145-193px-Write-a-Requirements-Document-Step-10.jpg",
      "stats": {
        "views": 202132,
        "last_updated": "Updated 1 year ago"
      }
    }
  ]
}
```

This endpoint retrieves the search results from wikihow.

### HTTP Request

`GET https://japi.rest/wikihow/v1/search?q=`

### Query Parameters

Parameter | Required | Description
--------- | -------- | -----------
q         | true     | The search query

## Information

```shell
curl "https://japi.rest/wikihow/v1/info/Write-Software-Documentation" \
  -H "Authorization: {API KEY}"
```

```javascript
const fetch = require('node-fetch'); // NodeJS users
const pageName = 'Write-Software-Documentation';
const data = fetch(`https://japi.rest/wikihow/v1/info/${pageName}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json())

console.log(data);
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": {
    "title": "How to Write Software Documentation",
    "description": "Good software documentation, whether a specifications document for programmers and testers, a technical document for internal users, or software manuals and help files for end users, helps the person working with the software understand its features and functions. Good software documentation is specific, concise, and relevant, providing all the information important to the person using the software.[1] X Research source Following are instructions on how to write software documentation for technical users and end users. ",
    "byline": {
      "name": "Author Info",
      "href": null
    },
    "last_updated": "January 19, 2021",
    "references": [
      { "ref_num": 1, "refrence": "https://clickhelp.com/software-documentation-glossary/software-documentation/" },
      { "ref_num": 2, "refrence": "https://www.gnu.org/software/emacs/manual/html_node/elisp/Documentation-Tips.html" },
      { "ref_num": 3, "refrence": "https://formidableforms.com/4-steps-to-creating-great-end-user-documentation/" },
      { "ref_num": 4, "refrence": "https://www.divio.com/blog/documentation/" },
      { "ref_num": 5, "refrence": "https://www.divio.com/blog/documentation/" },
      { "ref_num": 6, "refrence": "http://www.techscribe.co.uk/ta/how-to-write-user-documentation.htm" },
      { "ref_num": 7, "refrence": "http://www.techscribe.co.uk/ta/how-to-write-instructions.htm" },
      { "ref_num": 8, "refrence": "Rodney Ruff, Omaha, NE; experience as technical writer/help file author since 1997" }
    ],
    "sections": [
      {
        "prefix": "Method 1 of 2:",
        "headline": "Writing Software Documentation for Technical Users",
        "steps": [
          {
            "num": 1,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/5/57/Write-Software-Documentation-Step-1.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-1.jpg",
              "alt": "Image titled Write Software Documentation Step 1"
            },
            "content": "Determine what information needs to be included. Software specification documents serve as reference manuals for designers of the user interface programmers who write the code, and testers who verify that the software works as intended. The exact information depends on the program in question but may include any of the following:\n\nKey files within the application. This may include files created by the development team, databases accessed during the program's operation, and third-party utility programs.\nFunctions and subroutines. This includes an explanation of what each function or subroutine does, including its range of input values and output values.\nProgram variables and constants, and how they're used in the application.\nThe overall program structure. For a disc-based application, this may mean describing the program's individual modules and libraries, while for a Web application, this may mean describing which pages use which files."
          },
          {
            "num": 2,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/6/6f/Write-Software-Documentation-Step-2.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-2.jpg",
              "alt": "Image titled Write Software Documentation Step 2"
            },
            "content": "Decide how much of the documentation should be within the program code and how much should be separate from it. The more technical documentation is developed within the program's source code to begin with, the easier it will be to update and maintain along with the code, as well as to document various versions of the original application. At a minimum, documentation within the source code needs to explain the purpose of functions, subroutines, variables, and constants.[2]\n\tX\n\t\tResearch source\n\t\t\n\t\t\t\t\n\n\n\n\nIf the source code is particularly lengthy, it can be documented in the form of a help file, which can be indexed or searched with keywords. This is a particular advantage for applications where the program logic is fragmented over many pages and includes a number of supplemental files, as with certain Web applications.\nSome programming languages, such as Java and the .NET Framework (Visual Basic.NET, C #), have their own standards for documenting code. In these cases, follow the standards as to how much of the documentation should be included with the source code."
          },
          {
            "num": 3,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/8/85/Write-Software-Documentation-Step-3.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-3.jpg",
              "alt": "Image titled Write Software Documentation Step 3"
            },
            "content": "Choose the appropriate documentation tool. To some extent, this is determined by the language the code is written in, be it C++, C#, Visual Basic, Java, or PHP, as specific tools exist for these and other languages. In other cases, the tool to use is determined by the type of documentation required.\n\nWord-processing programs for Microsoft Word are adequate for creating separate text files of documentation, as long as the documentation is fairly short and simple. For long, complex text files, many technical writers prefer a documentation tool such as Adobe FrameMaker.\nHelp files for documenting source code can be produced with any help authoring tool, such as RoboHelp, Help and Manual, Doc-To-Help, MadCap Flare, or HelpLogix."
          }
        ]
      },
      {
        "prefix": "Method 2 of 2:",
        "headline": "Writing Software Documentation for End Users",
        "steps": [
          {
            "num": 1,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/8/85/Write-Software-Documentation-Step-4.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-4.jpg",
              "alt": "Image titled Write Software Documentation Step 4"
            },
            "content": "Determine the business reasons for your documentation. Although the functional reason for documenting software is to help users understand how to use the application, there are other reasons as well, such as assisting in marketing the software, enhancing the company image, and most notably, reducing technical support costs.[3]\n\tX\n\t\tResearch source\n\t\t\n\t\t\t\t\n\n\n In some cases, documentation is necessary to comply with certain regulations or other legal requirements.\nIn no case, however, should software documentation substitute for poor interface design. If an application screen requires reams of documentation to explain it, better to change the screen design to something more intuitive."
          },
          {
            "num": 2,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/3/35/Write-Software-Documentation-Step-5.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-5.jpg",
              "alt": "Image titled Write Software Documentation Step 5"
            },
            "content": "Understand the audience you're writing the documentation for. In most cases, software users have little knowledge of computers outside of the applications they use. There are several ways to determine how to address their needs with your documentation.\n\nLook at the job titles your prospective users hold. A system administrator is likely expert with a number of software applications, while a data entry clerk is more likely to know only the application he or she currently uses to enter data.\nLook at the users themselves. Although job titles generally indicate what people do, there can be considerable variation in how certain titles are used within a given organization. By interviewing prospective users, you can get a feel for whether your impressions of what their job title indicates are accurate or not.\nLook at existing documentation. Documentation for previous versions of software, as well as functional specifications, provide some indication as to what the user will need to know to use the program. Keep in mind, however, that end users are not as interested in how the program works as they are in what it can do for them.\nIdentify the tasks needed to do the job, and what tasks need to be done before those tasks can be done."
          },
          {
            "num": 3,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/5/5b/Write-Software-Documentation-Step-6.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-6.jpg",
              "alt": "Image titled Write Software Documentation Step 6"
            },
            "content": "Determine the appropriate format(s) for the documentation. Software documentation can be structured in 1 of 2 formats, the reference manual and the user guide. Sometimes, a combination of formats is the best approach.\n\nA reference manual format is devoted to explaining the individual features of a software application (button, tab, field, and dialog box) and how they work. Many help files are written in this format, particularly context-sensitive help that displays a relevant topic whenever a user clicks the Help button on a particular screen.[4]\n\tX\n\t\tResearch source\n\t\t\n\t\t\t\t\n\n\n\n\nA user guide format explains how to use the software to perform a particular task. User guides are often formatted as printed guides or PDFs, although some help files include topics on how to perform particular tasks. (These help topics are usually not context-sensitive, although they may be hyperlinked to from topics that are.) User guides often take the form of tutorials, with a summary of the tasks to be performed in the introduction and instructions given in numbered steps.[5]\n\tX\n\t\tResearch source"
          },
          {
            "num": 4,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/d/d9/Write-Software-Documentation-Step-7.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-7.jpg",
              "alt": "Image titled Write Software Documentation Step 7"
            },
            "content": "Decide what form(s) the documentation should take. Software documentation for end users can take 1 or several of many forms: printed manuals, PDF documents, help files, or online help. Each form is designed to show the user how to use each of the program's functions, whether in the form of a walkthrough or a tutorial; in the case of help files and online help, this may include demonstration videos as well as text and still graphics.\nHelp files and online help should be indexed and keyword-searchable to allow users to quickly find the information they're looking for. Although help file authoring tools can generate indexes automatically, it is often better to create the index manually, using terms users are likely to search for."
          },
          {
            "num": 5,
            "image": {
              "link": "https://www.wikihow.com/images/thumb/f/fd/Write-Software-Documentation-Step-8.jpg/aid1568971-v4-728px-Write-Software-Documentation-Step-8.jpg",
              "alt": "Image titled Write Software Documentation Step 8"
            },
            "content": "Choose the appropriate documentation tool. Printed or PDF user manuals can be written with a word-processing program like Word or a sophisticated text editor like FrameMaker, depending on their length and complexity. Help files can be written with a help authoring tool like RoboHelp, Help and Manual, Doc-To-Help, Flare, HelpLogix, or HelpServer."
          }
        ]
      }
    ]
  }
}
```

This endpoint retrieves a article's information.

### HTTP Request

`GET https://japi.rest/wikihow/v1/info/:title`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
title     | true     | The page title