# Open Drupal course template
Use this template to start a new Open Drupal course. Create a complete package with materials for both trainer and attendee.

Open Drupal materials are designed to be used by an knowlegable trainer to train others, and may therefore not be suitable for self study.

# Files

## Introduction
Directory: /intro
Contains information that can be used to promote a course, to inform (future) participants, to provide an outline and to set expectations.

## Set-up
Directory: /set-up
Contains instructions, code and data to set-up a course environment.

## Lessons
Directory: /lesson-1, /lesson-2, ...
Contains slides and other learning materials for the course. Broken down in lessons.
Has a corresponding lesson-*.html file with slides.

### Slides
Directory: /lesson-*/slides, /lesson-*/slides/assets
Markdown files with slides for this lesson. Images and other assets for this lesson are stored here too.

### Exercises
Directory: /lesson-*/exercises
Step-by-step instructions and source materials for exercises. Broken down like the lessons.

## Results
Directory: /result
The result of completed exercises. To be used as reference, study or copy/paste for those who got left behind.

## Slides
Directory: /slide-foundation
The reveal.js framework for slides with Open Drupal styling. Reveal.js is included as node package and stored in the repository to 