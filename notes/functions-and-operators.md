# Data Types

  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#logical-operators">Logical Operators</a></li>
    <li><a href="#string-functions-and-operators">String Functions and Operators</a></li>
    <li><a href="#json-functions-and-operators">JSON Functions and Operators</a></li>
    <li><a href="#numeric-functions-and-operators">Numeric Functions and Operators</a></li>
    <li><a href="#date-and-time-functions">Date and Time Functions and Operators</a></li>
  </ol>

## Logical Operators

_Logical operaters return as 1 (TRUE), 0 (FALSE), and NULL_

**AND** - Evaluates to 1 (TRUE) if all operands are nonzero and not NULL, to 0 (FALSE) if one or more operands are 0, otherwise NULL is returned.

**NOT** - Evaluates to 1 (TRUE) if the operand is 0, to 0 (FALSE) if the operand is nonzero, and NOT NULL returns NULL.

**OR** - When both operands are non-NULL, the result is 1 (TRUE) if any operand is nonzero, and 0 (FALSE) otherwise. With a NULL operand, the result is 1 (TRUE) if the other operand is nonzero, and NULL otherwise. If both operands are NULL, the result is NULL.

## Comparison Functions and Operators

**(>)** - Greater than operator

**(>=)** - Greater than or equal operator

**(<)** - Less than operator

**(<>)** - Not equal operator

**(<=)** - Less than or equal operator

**(<=>)** - NULL-safe equal to operator

**(=)** - Equal operator

**(BETWEEN ... AND ...)** - Whether a value is within a range of values

**COALESCE()** - Return the first non-NULL argument

**IS** - Test a value against a boolean

**IS NOT** - Test a value against a boolean

**IS NOT NULL** - NOT NULL value test

**IS NULL** - NULL value test

**LIKE** - Simple pattern matching

**NOT BETWEEN ... AND ...** - Whether a value is not within a range of values

**NOT IN()** - Whether a value is not within a set of values

**NOT LIKE** - Negation of simple pattern matching

**STRCMP()** - Compare two strings

## String Functions and Operators

**CHAR_LENGTH()** - Returns number of characters

**CONCAT()** - Return a concatenated string

**INSERT()** - Insert substring at specified position up to specified number of characters

**LENGTH()** - Return the length of a string in bytes

**LOWER()** - Return the argument of lowercase

**MATCH()** - Perform full-text search

**REPLACE()** - Replaces occurences of a specified string

**REVERSE()** - Reverse the characters in a string

**TRIM()** - Remove leading and trailing spaces

**UPPER()** - Convert to uppercase

## JSON Functions and Operators

**JSON_ARRAY()** - Create JSON Array

**JSON_ARRAY_APPEND()** - Append data to JSON document

**JSON_ARRAY_INSERT()** - Insert into JSON array

**JSON_EXTRACT()** - Return data from JSON document

**JSON_INSERT()** - Insert data into JSON document

**JSON_KEYS()** - Array of keys from JSON document

**JSON_LENGTH()** - Number of elements in JSON document

**JSON_PRETTY()** - Print a JSON document in human-readable format

**JSON_QUOTE()** - Quote JSON document

**JSON_REMOVE()** - Remove data from JSON document

**JSON_REPLACE()** - Replace values in JSON document

**JSON_SET()** - Insert data into JSON document

**JSON_TABLE()** - Return data from a JSON expression as a relational table

**JSON_TYPE()** - Type of JSON value

## Numeric Functions and Operators

**(\*)** - Multiplication operator

**(+)** - Addition operator

**(-)** - Minus operator

**(/)** - Division operator

**CEIL()** - Return the smallest integer value not less than the argument

**FLOOR()** - Return the largest integer value not greater than the argument

## Date and Time Functions

**ADDDATE()** - Add time values (intervals) to a date value

**ADDTIME()** - Add time

**CONVERT_TZ()** - Convert from one time zone to another

**CURDATE()** - Return the current date

**CURTIME()** - Return the current time

**DATE()** - Extract the date part of a date or datetime expression

**DATE_ADD()** - Add time values (intervals) to a date value

**DATE_FORMAT()** - Format date as specified

**DATE_SUB()** - Subtract a time value (interval) from a date

**DAY()** Synonym for DAYOFMONTH()

**DAYNAME()** - Return the name of the weekday

**DAYOFMONTH()** - Return the day of the month (0-31)

**DAYOFWEEK()** - Return the weekday index of the argument

**DAYOFYEAR()** - Return the day of the year (1-366)

**HOUR()** - Extract the hour

**MAKEDATE()** - Create a date from the year and day of year

**MAKETIME()** - Create time from hour, minute, second

**MINUTE()** - Return the minute from the argument

**MONTH()** - Return the month from the date passed

**MONTHNAME()** - Return the name of the month

**NOW()** - Return the current date and time

**SECOND()** - Return the second (0-59)

**STR_TO_DATE()** - Convert a string to a date

**UTC_DATE()** - Return the current UTC date

**UTC_TIME()** - Return the current UTC time

**UTC_TIMESTAMP()** - Return the current UTC date and time

**WEEK()** - Return the week number

**WEEKOFYEAR()** - Return the calendar week of the date (1-53)

**YEAR()** - Return the year

**YEARWEEK()** - Return the year and week
