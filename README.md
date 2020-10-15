# Visual Free Recall
Website built in javascript using the jsPsych library to test memory in a visual free recall memory task.
A running example of the most recent version of this script can be found here: https://6kopzqrw9w.cognition.run/?sequence=Demo

This script requires:
jsPsych 6.1, which can be downloaded here: https://github.com/jspsych/jsPsych/releases/tag/v6.1.0

If you want to run this program locally you will need to run a local web server so the GET request for the sequence file is not blocked.  I use the Web Server For Chrome app for debugging purposes, but you may want to do some research and decide what works best for you. When testing participants, we use a version of this program hosted on cognition.run

Once you have downloaded jsPsych 6.1, the FreeRecall.html file, and the Demo.txt experiment sequence, you can open the website in a web browser through your server and it should bring up task instructions.

This script implements a visual free recall task first described in Tulving and Colotla (1970, Cogn Psych), which was later used in word by Randy Engle's lab (e.g. Engle et al. 1999 J Exp Psych Gen). Each trial presents a list of words defined in the sequence file (a demo sequence file is included here) one at a time, with 750 ms per word and 250 ms inter-stimulus intervals. We used sequences of 12 words, but lists in the experiment sequence file can be any length. Each line corresponds to one list, with items within a list separated by commas. At the end of each list the program waits for the participant to click 'Click to start the next list'.  In our lab, we use this task in conjunction with a recorded video call so we can record verbal responses to each trial and score them offline.  Our lab also has specific procedures for recording and scoring data, which we will share on request (adam.bosen@boystown.org).
