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
title: Reading Questions 18
uid: 19b816de-bc6b-9a1d-a781-873c3813d1ef
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

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["Suppose data is drawn from a normal distribution with unknown mean $&mu;$ and unknown standard deviation.", "We make the following hypotheses:", kbr, "There are 100 points with a sample mean of 2 and sample variance of 36.", kp, ksp, ksp, "For a one-sample $t$-test let $H\_0$: $&mu; = 1$", ksp, "and", ksp, "$H\_A$: $&mu; > 1$."\]; wl(s.join(' ')); wl(kp) s = "(a) What is the value of the $t$ statistic?"; wl(s); wl(kbr); partName = problemNumber + " (a)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 5/3, buttonLabel, 0.01, kuseCorrectVal); wl(kp); s = "(b) How many degrees of freedom does the null distribution have?"; wl(s); wl(kbr); partName = problemNumber + " (b)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 99, buttonLabel, 0.01, kuseCorrectVal); wl(kp); s = "(c) What is the $p$-value for this test? Use R to compute your answer."; wl(s); wl(kbr); partName = problemNumber + " (c)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", .04937, buttonLabel, 0.002, kuseCorrectVal); wl(kp); s = "(d) At a significance level of $0.01$ do you reject the null hypothesis in favor of $H\_A$?"; wl(s); wl(kbr); partName = problemNumber + " (d)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "No"; var answerArray = \['Yes',correct\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); whr(kdivcol,kdivwid);