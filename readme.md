# Open Drupal course template
Use this template to start a new Open Drupal course. Create a complete package with materials for both trainer and attendee.

Open Drupal materials are designed to be used by an knowlegable trainer to train others, and may therefore not be suitable for self study.

## Contents
1. [Files](#files)
   1. [Introduction](#introduction)
   2. [Set-up](#setup)
   3. [Lessons](#lessons)
   4. [Slides](#slides)
   5. [Exercises](#exercises)
   6. [Results](#results)
2. [Slides setup](#slides-setup)

# <a href="#files">Files</a>
Use index.html for the slides of a small training course or as index for attendees of a larger course. lesson-1.html, lesson-2.html, etc for individual lessons of larger courses.

## <a href="#introduction">Introduction</a>
*Directory: /intro*  
Contains information that can be used to promote a course, to inform (future) participants, to provide an outline and to set expectations.

## <a href="#setup">Set-up</a>
*Directory: /set-up*  
Contains instructions, code and data to set-up a course environment.

## <a href="#lessons">Lessons</a>
*Directory: /lesson-1, /lesson-2, ...*  
Contains slides and other learning materials for the course. Broken down in lessons.
Has a corresponding lesson-*.html file with slides.

## <a href="#slides">Slides</a>
*Directory: /lesson-*/slides, /lesson-*/slides/assets*  
Markdown files with slides for this lesson. Images and other assets for this lesson are stored here too.

## <a href="#exercises">Exercises</a>
*Directory: /lesson-*/exercises*  
Step-by-step instructions and source materials for exercises. Broken down like the lessons.

## <a href="#results">Results</a>
*Directory: /result*  
The result of completed exercises. To be used as reference, study or copy/paste for those who got left behind.

# <a href="#slides-setup">Slides setup</a>
*Directory: /slide-foundation*  
The reveal.js framework is used for slides with Open Drupal styling. Reveal.js is included as node package and stored in the repository too.  

**Note for Chrome users:** You will need a server for showing the slides. You can use your local VM/Docker setup or use Node, but by default the repo does not contain a server solution. This is because the slide's contents are using markdown and Google Chrome does not allow for JS scripts to access local files by default.
Alternatively use Mozilla Firefox which currently has been tested and works to just open the slides directly in the browser.

If it's the first time the repo is used you will need to run `npm install` in this directory before you can use Gulp. Gulp is already setup to watch for changes, run `gulp` to automatically compile scss changes to the css. The task runner will open a new tab in your default browser and server the index.html file one directory above and use BrowserSync to serve CSS changes live.  
 You can update the sass stylesheet of the template by editing open-drupal.scss found in `/css/source`.
