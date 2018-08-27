# Vision Document

Template: https://jazz.net/help-dev/clm/index.jsp?re=1&topic=/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html&scope=null

##Introduction
###Purpose
This product will allow for students to take notes and turn them in through Canvas or Moodle.  This product will also generate questions based on the students notes.
###Scope
This product will be run on docker using a technology stack comprising of React, Node, and PostgreSQL.  All associated documentation will be done using Mkdocs. The product will be able to be used through Moodle and Canvas. The product will allow for students to take notes directly in Canvas.  Upon completion of notes, the product can generate questions based on the students notes that may be shareable at the instructors discretion. 
###Definitions
LTI - Learning Tools Interoperability
###References
###Overview
This document goes over the various business and planning aspects of this project/product.  It goes over the Product, Stakeholders/Users, Positioning, Constraints, and Documentation Requirements

##Positioning
###Business Opportunity
This project will improve the versatility of Canvas and the ways it can be used.  This adds new functionality to Canvas/Moodle that can help improve students' understanding of a topic.  This also allows Instructors to see what exactly their students are focusing on in their reading, allowing for the instructor to stress things in class that students may be missing in their reading.
###Problem Statement
Some instructors would like more insight into what their students are studying, so that the instructors can adjust to the speed of their class's understanding.  Students can take notes anywhere, but if they want to study by creating quizzes based on their notes, They must use a third party or do it on their own.
###Product Position Statement
This product will allow students to take notes and study quizzes that were created based on their notes.  It will also provide analytics for professors, such as what the most used keywords are in their class's notes.

##Stakeholders and Users
###Market Demographics
Canvas is used by every class and almost every extreacurricular organization on campus. It also has a reputation of being slow or unreliable at times (especially for grades).  Our focus is on user experience and reliability so that a student can easily and quickly access our LTI, and not lose any of their notes.  This also goes for instructors. They should be able to easily and quickly access our LTI and have accurate analytics information.
###Stakeholder Summary
Michael Aars - Project Sponsor/Owner/Client - is available for requirements questions as well as high level software questions

Development Team - will be creating the product to the requirements specifications.
###User Summary
Students - The typical student user that will utilize the product to turn in notes and use the quizzes it will generate

Instructors - The typical instructor that will utilize the product to view/grade notes and use the analytics based on the class's notes.
###User Environment
Students' environments are constantly changing as the move from classrooms to coffee shops to their homes. This product will need the ability to save the progress of a student's not taking session to match their mobility.  The sessions of use of this product could vary from minutes to hours.  Regardless, use of this product will require an internet connection, and can be used on any PC or MAC.
###Stakeholder Profiles
see summary?
###User Profiles
see summary?
###Key Stakeholder/User Needs
Cannot take notes in Canvas - User now takes notes in a word processor and uploads the document - User should be able to take and submit notes in Canvas

Creating quizzes based on notes is time consuming - Students take the time to create their own quizzes - After taking notes in Canvas, the user should be able to have access to questions that the product has generated after the user's notes have been submitted.
###Alternatives/Competition
The only alternatives to this utilize various tools: Microsoft Word/OneNote for note taking, Quizlet for generating quizzes(However, this requires questions and answers to be enterred manually)

##Product Overview
###Product Perspective
This product is an LTI extension to Canvas. It will require the user to already be logged into their institutions version of Canvas and all data will be shared between the product and Canvas utilizing REST Post calls.
###Capabilities Summary
Students can easily take/view/submit notes. The product will then generate a quiz based on these notes. This allows the students to do all of this in one place.
The Instructor gains insight on what the students are focusing on in their reading using the analytics provided by the product. 
###Assumptions and Dependencies
-Uses all of Canvas/Moodle system requirements (ex: OS of MAC and PC)

-Requires users to be users with Canvas/Moodle
###Cost and Pricing
-minimal?
###Licensing and Installation
Unknown

##Product Features
###Note Taker
Allows for a drag and drop style of adding to the page of taking notes.  This allows for the system to understand the structure of a user's notes and easily create a quiz based on them.  Also will allow for easy reading by others including the instructor if grades are taken. Users will also be able to save their progress as they take notes should they need multiple sessions to finish.
###Quiz Generator
Quizzes are only generated after submitting the final version of notes.  This allows for the same quiz to not be generated multiple times.  Is viewable only to the user that submitted the notes, and can be taken as many time as they like.
###Analytics
A master version is available to the Instructor to view various analytics of the notes to answer questions such as which keywords are being used most, what sections of the book/chapter are being heavily noted, etc.

##Constraints
Must be portable to Canvas and Moodle

##Quality Ranges
Must be accessible to all Instructors. Must be accessible to all students whose instructors have assigned the use of the product.

##Precedence and Priority
Number one priority is security. Notes should only be viewable to those that have ben given explicit access. Notes should also be reliably saved and accessible to the appropriate users.

##Other Product Requirements
###Applicable Standards
RESTful API calls

Windows/MAC OS

###System Requirements
???
###Performance Requirements
???
###Environmental Requirements
Internet Connection for reliable saving of note taking progress.

##Documentation Requirements
###Release Notes, Readmes
See Mkdocs Documentation
###Online Help
See Mkdocs Documentation
###Installation Guides
See Mkdocs Documentation