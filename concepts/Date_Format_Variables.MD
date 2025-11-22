# Time Format Variables

Date and time variables

%c	The date and time in the current locale's format as defined by the server's operating system. For example, Thu Jul 18 09:30:00 2019 for US English on Linux.

%+	The date and time with time zone in the current locale's format as defined by the server's operating system. For example, Thu Jul 18 09:30:00 PDT 2019 for US English on Linux.

__Time variables__

%Ez	Splunk-specific, timezone in minutes.

%f	Microseconds as a decimal number.

%H	Hour (24-hour clock) as a decimal number. Hours are represented by the values 00 to 23. Leading zeros are accepted but not required.

%I	Uppercase "i". Hour (12-hour clock) with the hours represented by the values 01 to 12. Leading zeros are accepted but not required. Use with %p to specify AM or PM for the 12-hour clock.

%k	Like %H, the hour (24-hour clock) as a decimal number. Leading zeros are replaced by a space, for example 0 to 23.

%M	Minute as a decimal number. Minutes are represented by the values 00 to 59. Leading zeros are accepted but not required.

%N	The number of subsecond digits. The default is %9N. You can specify %3N = milliseconds, %6N = microseconds, %9N = nanoseconds.

%p	AM or PM. Use with %I to specify the 12-hour clock for AM or PM. Do not use with %H.

%Q	The subsecond component of a UTC timestamp. The default is milliseconds, %3Q. Some valid values are: %3Q = milliseconds, with values of 000-999, %6Q = microseconds, with values of 000000-999999, %9Q = nanoseconds, with values of 000000000-999999999

%S	Second as a decimal number, for example 00 to 59.

%s	The UNIX Epoch Time timestamp, or the number of seconds since the Epoch: 1970-01-01 00:00:00 +0000 (UTC). For example the UNIX epoch time 1484993700 is equal to Tue Jan 21 10:15:00 2020.

%T	The time in 24-hour notation (%H:%M:%S). For example 23:59:59.

%X	The time in the format for the current locale. For US English the format for 9:30 AM is 9:30:00.

%Z	The timezone abbreviation. For example EST for US Eastern Standard Time.

%z	The timezone offset from UTC, in hour and minute: +hhmm or -hhmm. For example, for 5 hours before UTC the values is -0500 which is US Eastern Standard Time. Examples: Use %z to specify hour and minute, for example -0500, Use %:z to specify hour and minute separated by a colon, for example -05:00, Use %::z to specify hour minute and second separated with colons, for example -05:00:00, Use %:::z to specify hour only, for example -05

%%	A literal "%" character.

Note: To parse timestamps with GMT and an offset in data that you upload using Add Data, such as Fri Apr 29 2022 23:45:22 GMT-0700, you might need to use %:Z to capture both the timestamp and the offset.

Date variables

%F	Equivalent to %Y-%m-%d (the ISO 8601 date format).

%x	The date in the format of the current locale. For example, 7/13/2019 for US English.

Specifying days and weeks

%A	Full weekday name. (Sunday, ..., Saturday)

%a	Abbreviated weekday name. (Sun, ... ,Sat)

%d	Day of the month as a decimal number, includes a leading zero. (01 to 31)

%e	Like %d, the day of the month as a decimal number, but a leading zero is replaced by a space. (1 to 31)

%j	Day of year as a decimal number, includes a leading zero. (001 to 366)

%V (or %U)	Week of the year. The %V variable starts the count at 1, which is the most common start number. The %U variable starts the count at 0.

%w	Weekday as a decimal number. (0 = Sunday, ..., 6 = Saturday)


Specifying months

%b	Abbreviated month name. (Jan, Feb, etc.)

%B	Full month name. (January, February, etc.)

%m	Month as a decimal number. (01 to 12). Leading zeros are accepted but not required.


Specifying year

%C	The century as a 2-digit decimal number.

%g	The ISO 8601 date format for year as a 2-digit decimal number, without the century. (00 to 99). For example, 25.

%G	The ISO 8601 date format for year with the century as a 4-digit decimal number that corresponds to the ISO week number (see %V). For example, 2025. %G uses the year that is associated with the ISO week number; if the ISO week number belongs to the previous or next year, %G specifies that year.

%y	Year as a decimal number, without the century. (00 to 99). Leading zeros are accepted but not required.

%Y	Year as a decimal number with the century. For example, 2025.
