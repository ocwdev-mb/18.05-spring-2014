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
title: Reading Questions 22
uid: f265cfd1-77f6-2963-d0c5-1227c4e2dee5
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

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["Suppose you have 9 data points drawn from N$(&mu;,1)$ with sample mean $\\\\ov{x} = 3$.", kbr, "What is the 95% confidence interval for the mean $&mu;$?", kp, "(Use the approximation 2 instead of 1.96 for $z\_{0.025}$.)"\]; wl(s.join(' ')); wl(kp); s = "(1.i) Give the lower limit:"; wl(s); wl(kbr); partName = problemNumber + ".i"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 2.3333, buttonLabel, 0.002, kuseCorrectVal); wl(kp); s = "(1.ii) Give the upper limit:"; wl(s); wl(kbr); partName = problemNumber + ".ii"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 3.6667, buttonLabel, 0.002, kuseCorrectVal); wl(kp); whr(kdivcol,kdivwid);

//Problem 2 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "Suppose you have 9 data points drawn from $N(&mu;,&sigma;^2)$. Suppose that \[4.2, 6,8\] is a 95% confidence interval for $&mu;$."; wl(s); wl(kp); s = "What is the probability that $4.2 &le; &mu; &le; 6.8$?"; wl(s); wl(kbr); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "Frequentists do not compute probabilities of hypotheses"; var answerArray = \["0.95", "0.05", "0.95/3", correct\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); whr(kdivcol,kdivwid);