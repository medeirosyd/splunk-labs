# Time Modifiers

earliest	earliest=[+|-] <time_integer><time_unit>@<time_unit>	Specify the earliest _time for the time range of your search. Use earliest=1 to specify the UNIX epoch time 1, which is UTC January 1, 1970 at 12:00:01 AM. 
Use earliest=0 to specify the earliest event in your data.

_index_earliest	_index_earliest=[+|-] <time_integer><time_unit>@<time_unit>	Specify the earliest _indextime for the time range of your search.

_index_latest	_index_latest=[+|-] <time_integer><time_unit>@<time_unit>	Specify the latest _indextime for the time range of your search.

latest	latest=[+|-] <time_integer><time_unit>@<time_unit>	Specify the latest time for the _time range of your search.

now	now() or now	Refers to the current time. If set to earliest, now() is the start of the search.

time	time()	In real-time searches, time() is the current machine time.

## Time unit	Valid unit abbreviations

subseconds	----> microseconds (us), milliseconds (ms), centiseconds (cs), or deciseconds (ds)

second	----> 	s, sec, secs, second, seconds

minute	----> 	m, min, mins, minute, minutes

hour	----> 	h, hr, hrs, hour, hours

day	----> 	d, day, days

week	----> 	w, week, weeks

month	----> 	mon, month, months

quarter	----> 	q, qtr, qtrs, quarter, quarters

year	----> 	y, yr, yrs, year, years

## Sample

...earliest=1 latest=now()

...earliest=@w0

...earliest=-5d@w1 latest=@w6

...earliest="11/15/2022:20:00:00" latest="11/22/2022:20:00:00"

...(earliest="9/23/2022:17:00:00" latest="9/23/2022:18:00:00")  OR  (earliest="9/23/2022:19:00:00" latest="9/23/2022:20:00:00")

...((earliest=-24h latest<@d) OR (earliest>=@d+1h))

## Other time modifiers

daysago	daysago=<int>	Search events within the last integer number of days.

enddaysago	enddaysago=<int>	Set an end time for an integer number of days before Now.

endhoursago	endhoursago=<int>	Set an end time for an integer number of hours before Now.

endminutesago	endminutesago=<int>	Set an end time for an integer number of minutes before Now.

endmonthsago	endmonthsago=<int>	Set an end time for an integer number of months before Now.

endtime	endtime=<string>	Search for events before the specified time (exclusive of the specified time). Use timeformat to specify how the timestamp is formatted.

endtimeu	endtimeu=<int>	Search for events before the specific UNIX time.

hoursago	hoursago=<int>	Search events within the last integer number of hours.

minutesago	minutesago=<int>	Search events within the last integer number of minutes.

monthsago	monthsago=<int>	Search events within the last integer number of months.

searchtimespandays	searchtimespandays=<int>	Search within a specified range of days, expressed as an integer.

searchtimespanhours	searchtimespanhours=<int>	Search within a specified range of hours, expressed as an integer.

searchtimespanminutes	searchtimespanminutes=<int>	Search within a specified range of minutes, expressed as an integer.

searchtimespanmonths	searchtimespanmonths=<int>	Search within a specified range of months, expressed as an integer.

startdaysago	startdaysago=<int>	Search the specified number of days before the present time.

starthoursago	starthoursago=<int>	Search the specified number of hours before the present time.

startminutesago	startminutesago=<int>	Search the specified number of minutes before the present time.

startmonthsago	startmonthsago=<int>	Search the specified number of months before the present time.

starttime	starttime=<timestamp>	Search from the specified date and time to the present, inclusive of the specified time.

starttimeu	starttimeu=<int>	Search for events starting from the specific UNIX time.

timeformat	timeformat=<string>	Set the timeformat for the starttime and endtime modifiers. By default: timeformat=%m/%d/%Y:%H:%M:%S
