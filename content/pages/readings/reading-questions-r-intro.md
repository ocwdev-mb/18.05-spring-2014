---
content_type: page
description: This section provides an interactive answer checker for the reading questions
  associated with an assigned reading.
learning_resource_types:
- Readings
ocw_type: CourseSection
parent_title: Readings
parent_type: CourseSection
parent_uid: 579c055a-ccb4-eb7e-bb6b-f294146b45a5
title: Reading Questions - R Intro
uid: 6bf95815-6f93-6518-4810-f71b343ad1a3
video_files:
  video_thumbnail_file: null
video_metadata:
  youtube_id: null
---

Reading Questions Answer Checker
--------------------------------

To check your answers put them in the appropriate box and click the 'Check' button. Every checker box can do arithmetic and calculate standard functions (see {{% resource_link 758ceee0-d290-5d7c-5072-7d458581a3b3 "calculator help" %}}). If you give decimal answers, give them to at least 3 decimal places.

As you work you should have pencil and paper handy for calculations and thinking!

Note: some questions ask for a formula. For the checker we ask you to plug a value into the formula. For your pset you still need to give the whole formula.

//DEBUG PARAMETERS //Because we don't show solutions for pset checkers we use //this to give a showanswer button during the debugging phase var debugans = undefined; //release //var debugans = kDebugAnswer; //debug problemNumber = 0; wl("\<h3>Calculator\</h3>"); writecalculator("psetcheckcalcid", "Calculate"); whr(kdivcol,kdivwid);

At this point you should have {{% resource_link a4d4ed52-37df-946d-c2b1-9d114f44c277 "installed R and R studio" %}}. If not, you should do that now.

The first thing to do with R is to make sure you can start it and then we will do some simple calculations. Give your answers to at least 2 decimal places of accuracy. Go ahead and start R Studio. You should see a window with 4 panes. The **command prompt** (the >) is in the bottom left window.

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); wl(kp); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["At the command prompt type the command", kp, rcmdna("2 + 3"), kp, "Hit return and enter the result here."\]; wl(s.join(' ')); wl(kp); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 5, buttonLabel, 0.001, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 2 problemNumber++; wl(problemheader(problemNumber)); wl(kp); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["Do the following computations using R.", kbr, "(Enter your answers in the boxes.)"\]; wl(s.join(' ')); wl(kp); wl(rcmdna("2\*3")); wl(kbr) partName = problemNumber + " (a)" problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 6, buttonLabel, 0.01, kuseCorrectVal); wl(kp) wl(rcmdna("2^3")); wl(kbr) partName = problemNumber + " (b)" problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 8, buttonLabel, 0.01, kuseCorrectVal); wl(kp) wl(rcmdna("3.14^3.14")); wl(kbr) partName = problemNumber + " (c)" problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 36.338, buttonLabel, 0.01, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 3 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["Use R to do the following computation.", kbr, "(Enter your answer to 2 decimal places in the box.)"\]; wl(s.join(' ')); wl(kp); wl(rcmdna("100\*mean(sin(30:87))")); wl(kbr) partName = problemNumber problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", -2.215, buttonLabel, 0.01, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 4 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["Now we'll do our first random simulation. Don't worry if you", "don't fully understand the commands. We will explain them in", "the first tutorial. ", kp, "In order to simulate counting the number of heads in 1000 tosses of", "a fair coin give the following sequence of commands.", kp, "(Hit return after each one)."\]; wl(s.join(' ')); wl(kp); wl(rcmdna("x = rbinom(1000,1,.5)")); wl(kbr) wl(rcmdna("total = sum(x)")); wl(kp); wl("You can use the up arrow to go back and run the commands again. You should get a different total."); wl(kp); wl("Give the value of the total number of heads for one of your simulations."); wl(kbr) partName = problemNumber problemName = "prob" + partName; buttonLabel = "Check problem " + partName; s = "Expect the answer will be between 450 and 550"; writeNumericBox(partName+"id", 500, buttonLabel, 460, s); whr(kdivcol,kdivwid);