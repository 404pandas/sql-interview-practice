# Data Types

  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#numeric-data">Numeric Data</a></li>
    <li><a href="#string-data">String Data</a></li>
    <li><a href="#date-data">Date Data</a></li>
    <li><a href="#other-data">Other Data</a></li>
  </ol>

## Numeric Data

- **INT:** Standard interger values. Can be TINYINT, INT, MEDIUMINT, and LONGINT.

-- Example: TINYINT = up to 255 bytes -- INT = up to 65,535 bytes -- MEDIUMINT = up to 16,777,215 bytes -- LONGINT = up to 4,294,967,295 bytes

- **FLOAT & DOUBLE:** Approximate numeric data values. _(Deprecated)_

## String Data

- **VARCHAR:** Length of 0 to 65,535. Doesn't retain trailing spaces.

-- Example: VARCHAR(30) defines 30 characters.

-- Example: 'COSSETTE' for VARCHAR(30) is stored and retrieved as 'COSSETTE'

- **TEXT**: Non-Binary large object. Can be TINYTEXT, TEXT, MEDIUMTEXT, and LONGTEXT.

-- Example: TINYTEXT = up to 255 bytes -- TEXT = up to 65,535 bytes -- MEDIUMTEXT = up to 16,777,215 bytes -- LONGTEXT = up to 4,294,967,295 bytes

- **CHAR:** Fixed characters that are declared when table is created. Length of 0 to 255. Retain trailing spaces when stored to specified length.

-- Example: CHAR(30) defines 30 characters.

-- Example: 'COSSETTE' for CHAR(30) is stored as 'COSSETTE '. 'COSSETTE' is retrieved as 'COSSETTE'.

- **ENUM:** String object with value chosen from list of permitted values that are stated explicitly in the column specification at table creation time

-- Example: Choosing between 'toy' 'herding' 'sporting' 'working' 'hound' 'terrier' 'non-sporting'

- **SET:** Max of 64 members. Can have 0 or more values. Multiple set members are specified by (,) commas.

-- Example: '' 'black' 'cream' 'black,cream' 'blue' 'fawn' 'spotted' 'chestnut' 'red' 'brown' 'brindle' 'gold' 'white' 'white,brown,black' 'brown' 'gray' 'yellow'

- **BLOB:** Binary large object. Can be TINYBLOB, BLOB, MEDIUMBLOB, and LONGBLOB.

-- Example: TINYBLOB = up to 255 bytes -- BLOB = up to 65,535 bytes -- MEDIUMBLOB = up to 16,777,215 bytes -- LONGBLOB = up to 4,294,967,295 bytes

## Date Data

- **DATE:** Values with date but no time. 'YYYY-MM-DD' Range of '1000-01-01' to '9999-12-31'

-- Example: '2023-10-18'

- **DATETIME:** Values that contain date and time. 'YYYY-MM-DD hh:mm:ss' Range of '1000-01-01 00:00:00' to '9999-12-31 23:59:59'

-- Example: '2023-10-18 11:55:00'

- **TIMESTAMP:** Values that contain both date and time. Uniquely converts current time zone to UTC for storage, then back to current time zone for retrieval.

-- Example: '2020-01-01 13:10:10' stores as '2020-01-01 18:10:10'

- **TIME:** Values that contain time. 'hh:mm:ss' or 'hhh:mm:ss' Range of '-838:59:59' to '838:59:59' _do not abbreviate_

-- Example: '11:55:00'

- **YEAR:** Represents year values. 'YYYY' Range of '1901' to '2155' or '0000'

-- Example: (4 digit string) '2023', (4 digit numbers) 2023, (1- or 2- digit string) '0' or '23', (1- or 2- digit numbers) 0 or 23

## Other Data

- **BINARY & VARBINARY:** Similar operations to CHAR and VARCHAR, but stores as binary strings. Comparison and sorting are based on the numeric values of the bytes in the values.

--Example: BINARY(7) column 'Nugget ' becomes 'Nugget \0'

- **JSON:** Allows JavaScript Object Notation documents. Automatic validation. JSON_ARRAY, JSON_OBJECT, JSON_QUOTE

--Example: JSON_OBJECT('owner_name', 'Mary', 'dog_name', 'Cossette')
