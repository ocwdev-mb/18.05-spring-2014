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
title: Reading Questions 5c
uid: 3876a769-ff7d-4764-1b94-468f23f85fc3
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

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "Suppose $X$ is a continuous random variable with pdf $f(x)$."; wl(s); wl(kp); s = \["Let $Z$ be a standard normal random variable.", kbr, "Use the R function " + rtext('pnorm') + " to compute each of the following.", kbr, "(Give 3 decimal places of accuracy.)"\]; wl(s.join(' ')); wl(kp); s = "(a) $P(Z \< 1.5)$."; wl(s) wl(kp) partName = problemNumber + " (a)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 0.93319, buttonLabel, 0.001, kuseCorrectVal); wl(kp); s = "(b) $P(-1 \< Z \< 1)$."; wl(s); wl(kp); partName = problemNumber + " (b)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", .68269, buttonLabel, 0.001, kuseCorrectVal); wl(kp); whr(kdivcol,kdivwid);