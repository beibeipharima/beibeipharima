SET Number TO 3 
 SEND "enter guess" TO DISPLAY
 RECEIVE Guess FROM KEYBOARD
 IF Guess > 10 
   SEND "guess too high" TO DISPLAY
 ELSE 
   IF Guess = Number 
     SEND "Correct!" TO DISPLAY 
   ELSE
     SEND "Bad luck! The correct number is" + Number
   END IF
 END IF
