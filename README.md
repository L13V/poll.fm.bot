# Poll.js Voter

This is pretty easy to use.  Just download the Python script, and customize the variables for what form/answer/number of votes.
Be sure to add your tor hash password found in torrc file.  

It needs Python 2.7.6. // Updated to Python 3.
Also be sure to do pip install requests and pip install TorRequest

### Disclaimer
This script will **may not -- I have not tested it with new tor functionality** work on polls that do not allow multiple votes from one person.  The useragents and proxy settings will help try and mask your mass voting, but they will not get you around IP blocks.  If someone wants to give a shot at forking this and adding that functionality, I will be happy to merge it in.

### Example
You want to vote on this poll: https://poll.fm/13523858 for the answer "Melanie Castellanos, Coral Park", and you want to vote 1000 times.  The poll_id comes from the url: <code>https://poll.fm/<b>13523858</b>/</code>. The answer_id comes from the looking at the source code for the associated checkbox: <code>\<input type="radio" name="PDI_answer" id="PDI_answer60463245" value="**60463245**"></code>.


Thus, you would want the variables to be set to:
```
poll_id = 13523858
answer_id = 60463245
number_of_votes = 1000
```
