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
title: Reading Questions 1b
uid: caf31075-1097-3b4e-ce1a-70518e49f2e9
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

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; s = "How many ways can you choose 4 kittens from a litter of 9?"; wl(s); wl(kp); var buttonLabel = "Check problem " + problemNumber; writeNumericBox(problemNumber+"id", 126, buttonLabel, 0.001, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 2 problemNumber++; wl(problemheader(problemNumber)); var s s = "How many sequences of 8 nucleotides can be made using any of the 4 nucleotides A, C, G, T at each place of the sequence?" wl(s); wl(kp); var buttonLabel = "Check problem " + problemNumber; writeNumericBox(problemNumber+"id", 65536, buttonLabel, 0.001, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 3 problemNumber++; wl(problemheader(problemNumber)); s = \["Suppose a sequence of 8 nucleotides contains 2 each of A, C, G, T.", kp, "How many such sequences are there?"\]; wl(s.join(' ')); wl(kbr); var problemName = "prob" + problemNumber; var buttonLabel = "Check problem " + problemNumber; var correct = 2520 var answerArray = \[70,1120,correct,37800\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); whr(kdivcol,kdivwid);