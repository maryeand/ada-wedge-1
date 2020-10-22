# ADA Fall 2020 Wedge Project

All files are added to the repo. 
The Submission file includes which files are for which part of the assginment, the GBQ queries results, and my reflection.

## Feedback

Thanks for the reflections. I'm glad that you felt a sense of community despite the pandemic-isolation of the
semester. Your queries all look spot on. 

Your cleaning file looks good. One note would be to make sure that none of your lines are more than 
80 characters wide (you have a couple of comments that run over). Keeping that width makes your
code more readable across devices. The code looks clean, though. Similarly, everything looks good
in the GBQ upload. 

For the owner sample, if this were a normal submission I'd ask you to resubmit without that large list
printed to the screen. Since this project is such a bear, let's not worry about it, but remember to 
check the submission guidelines (under the assignment section of Moodle) to help you get your code
shipshape. The actual code looks great.

For part 3, you start like this: 
```
path_to_files = 'C:\\Users\\meand\\Documents\\Grad School\\Fall2020\\Applied Data Analytics\\Wedge\\ada-wedge\\bigwedge_clean\\'
clean_wedge = os.listdir("bigwedge_clean")
```
You never use either of these variables, though there was no error, so presumably `bigwedge_clean` is 
inside the same directory. This is fine, but by this point in the semester I'd expect you to be a 
bit more in control on where stuff sits and how to access it. I'm guessing these lines came over in a
copy-paste from Part 2. Anyway, it looks a bit weird to have code that doesn't do anything in a final
submission. Generally this code looks fine, although you could make it a smidge more efficient by just 
having one line that makes the connection to the DB:
```
db = sqlite3.connect("WedgeTask3.db")# connect to the WedgeTask 3 database
cur = db.cursor()
```
Be on the lookout for places where you do the same thing over and over again. Computers are good 
at that, but humans are error prone. 

None of these rise to the level of needing a revision, though. Congratulations, you made it 
through the Wedge project!






