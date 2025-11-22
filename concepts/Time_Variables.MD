# Time Variables

%Ez	Splunk-specific, timezone in minutes.

%f	Microseconds as a decimal number.

%H	Hour (24-hour clock) as a decimal number. Hours are represented by the values 00 to 23. Leading zeros are accepted but not required.

%I	Uppercase "i". Hour (12-hour clock) with the hours represented by the values 01 to 12. Leading zeros are accepted but not required. Use with %p to specify AM or PM for the 12-hour clock.

%k	Like %H, the hour (24-hour clock) as a decimal number. Leading zeros are replaced by a space, for example 0 to 23.

%M	Minute as a decimal number. Minutes are represented by the values 00 to 59. Leading zeros are accepted but not required.

%N	The number of subsecond digits. The default is %9N. You can specify %3N = milliseconds, %6N = microseconds, %9N = nanoseconds.

%p	AM or PM. Use with %I to specify the 12-hour clock for AM or PM. Do not use with %H.

%Q	The subsecond component of a UTC timestamp. The default is milliseconds, %3Q. Some valid values are:   %3Q = milliseconds, with values of 000-999    %6Q = microseconds, with values of 000000-999999   %9Q = nanoseconds, with values of 000000000-999999999

%S	Second as a decimal number, for example 00 to 59.

%s	The UNIX Epoch Time timestamp, or the number of seconds since the Epoch: 1970-01-01 00:00:00 +0000 (UTC). For example the UNIX epoch time 1484993700 is equal to Tue Jan 21 10:15:00 2020.

%T	The time in 24-hour notation (%H:%M:%S). For example 23:59:59.

%X	The time in the format for the current locale. For US English the format for 9:30 AM is 9:30:00.

%Z	The timezone abbreviation. For example EST for US Eastern Standard Time.

%z	The timezone offset from UTC, in hour and minute: +hhmm or -hhmm. For example, for 5 hours before UTC the values is -0500 which is US Eastern Standard Time. Examples:

Use %z to specify hour and minute, for example -0500

Use %:z to specify hour and minute separated by a colon, for example -05:00

Use %::z to specify hour minute and second separated with colons, for example -05:00:00

Use %:::z to specify hour only, for example -05

%%	A literal "%" character.
