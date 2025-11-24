Working_With_Time Quiz

Question
01/08
@timeUnit will always round up and go forward through time.

FALSE  ---------- CORRECT ANSWER!

TRUE


Question
02/08
Choose the search that will sort events into one minute groups. Select all that apply.

| bin span=1minute

| bin _time span=1mins  ---------- CORRECT ANSWER!

| bin span=1minutes

| bin _time span=1m  ---------- CORRECT ANSWER!


Question
03/08
Which of the following are default time fields? Select all that apply.

date_year ---------- CORRECT ANSWER!

date_hour ---------- CORRECT ANSWER!

date_day

date_mday ---------- CORRECT ANSWER!





Question
04/08
The _______ and _______ time modifiers will override the time range picker in a historical report.

last

first

earliest ---------- CORRECT ANSWER!

latest ---------- CORRECT ANSWER!




Question
05/08
When using the following search arguments, what will be returned?  | timechart count span=1h

chart of events in 1 hour chunks ---------- CORRECT ANSWER!

events with a duration of 1 hour

events in the last 24 hours



Question
06/08
What will the strftime function return when using the %H argument with the _time field? Select all that apply.

time of raw event in UTC

hour of the event generated at index time

convert the hour into your local time based on your time zone setting of your Splunk web sessions ---------- CORRECT ANSWER!



Question
07/08
Using earliest=-30d@d latest=@d is how to return results from 30 days ago up until the time the search was executed.

TRUE

FALSE  ---------- CORRECT ANSWER!




Question
08/08
date_time always reflects your local time zone and not the time/date from raw events.

FALSE ---------- CORRECT ANSWER!

TRUE




