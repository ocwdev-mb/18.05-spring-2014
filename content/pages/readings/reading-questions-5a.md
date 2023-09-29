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
title: Reading Questions 5a
uid: e4f84c80-4eda-51c1-cbe5-b150bae38f18
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

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["A random variable $X$ takes values $1$, $2$ and $4$ with probabilities $0.2$, $0.3$ and $0.5$ respectively.", kp, "What is Var$(X)$?"\]; wl(s.join(' ')); wl(kp); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 1.56, buttonLabel, 0.01, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 2 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "Suppose $X$ has mean 2 and variance 3. Compute the following." wl(s); wl(kp); s = \["(a) Var$(3X)$"\]; wl(s.join(' ')); wl(kp); partName = problemNumber + " (a)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 27, buttonLabel, 0.01, kuseCorrectVal); wl(kp); s = \["(b) Var$(3X+8)$"\]; wl(s.join(' ')); wl(kp); partName = problemNumber + " (b)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 27, buttonLabel, 0.01, kuseCorrectVal); wl(kp); s = \["(c) $E(X^2)$"\]; wl(s.join(' ')); wl(kp); partName = problemNumber + " (c)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 7, buttonLabel, 0.01, kuseCorrectVal); whr(kdivcol,kdivwid);

//Problem 3 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "For the same random variable as in problem 2."; wl(s) wl(kp); s = "(a) Var$(X^2)$ = "; wl(s) wl(kbr) partName = problemNumber + " (a)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "Cannot be computed from the information given" var answerArray = \["13", "9", "5", correct\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); s = "(b) Can $X$ take negative values?"; wl(s) wl(kbr) partName = problemNumber + " (b)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "Yes" var answerArray = \[correct, "No"\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); whr(kdivcol,kdivwid);

//Problem 4 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = \["(a) True or false:", kp, "$E(X+Y) = E(X) + E(Y)$ for any random variables $X$ and $Y$."\]; wl(s.join(' ')); wl(kbr); partName = problemNumber + " (a)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "True" var answerArray = \[correct, "False"\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); s = \["(b) True or false:", kp, "Var$(X+Y) = $Var$(X) + $Var$(Y)$ for any random variables $X$ and $Y$."\]; wl(s.join(' ')); wl(kbr); partName = problemNumber + " (b)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "False" var answerArray = \["True",correct\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); whr(kdivcol,kdivwid);

//Problem 5 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "$X &#x223c; $ Bernoulli(.8). What is the standard deviation of $X$?"; wl(s) wl(kp); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 0.4, buttonLabel, 0.01, kuseCorrectVal); wl(kp); whr(kdivcol,kdivwid);