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
title: Reading Questions 5d
uid: 311ca439-afe7-5774-6b72-61ed1efc2773
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

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["Suppose $X &#x223c;$ Uniform$(0,1)$ and $Y = X^3$. The pdf for $Y$ is"\]; wl(s.join(' ')); wl(kbr); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "$1/3 y^{-2\\3}$"; var answerArray = \["$3y^2$", "$y^3$", "$4/3 y^{1\\/3}$", correct\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); whr(kdivcol,kdivwid);