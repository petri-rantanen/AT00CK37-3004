# JavaScript Utility Library

A dependency-free JavaScript utility library.

All modules are written in ES Modules format and documented with JSDoc.

---

## Project Structure

src/
├── arrays/
├── collections/
├── conversion/
├── dates/
├── logic/
├── math/
├── misc/
├── objects/
├── strings/
└── - validation/


---

## Functions

The utility library contains 10 modules (arrays, collections, conversion, dates, logic, math, misc, objects, strings, validation).

Functions for these modules are listed below.

The format of the documentation is:
- FILE_NAME FUNCTION_NAME(INPUTS) -> OUTPUTS: BRIEF_DESCRIPTION_OF_THE_FUNCTION

### Arrays

- arrays/basicArrayUtils.js clone(arr) -> Array: Creates a shallow copy of an array
- arrays/basicArrayUtils.js first(arr) -> any | undefined: Returns the first element of an array
- arrays/basicArrayUtils.js isEmpty(arr) -> boolean: Checks whether an array is empty
- arrays/basicArrayUtils.js last(arr) -> any | undefined: Returns the last element of an array

- arrays/filterArrayUtils.js onlyEven(arr) -> number[]: Returns only even numbers from an array
- arrays/filterArrayUtils.js onlyOdd(arr) -> number[]: Returns only odd numbers from an array
- arrays/filterArrayUtils.js removeDuplicates(arr) -> Array: Removes duplicate values from an array
- arrays/filterArrayUtils.js removeFalsy(arr) -> Array: Removes all falsy values from an array

- arrays/searchArrayUtils.js contains(arr, value) -> boolean: Checks whether an array contains a value
- arrays/searchArrayUtils.js count(arr, value) -> number: Counts the occurrences of a value in an array
- arrays/searchArrayUtils.js indexOf(arr, value) -> number: Returns the index of a value or -1 if not found
- arrays/searchArrayUtils.js unique(arr) -> Array: Returns an array of unique values

- arrays/sortArrayUtils.js reverseArray(arr) -> Array: Reverses the order of elements in an array
- arrays/sortArrayUtils.js sortAscending(arr) -> number[]: Sorts numbers in ascending order
- arrays/sortArrayUtils.js sortDescending(arr) -> number[]: Sorts numbers in descending order
- arrays/sortArrayUtils.js sortStrings(arr) -> string[]: Sorts strings alphabetically

- arrays/transformArrayUtils.js doubleNumbers(arr) -> number[]: Doubles all numeric values in an array
- arrays/transformArrayUtils.js flattenOneLevel(arr) -> Array: Flattens a nested array by one level
- arrays/transformArrayUtils.js squareNumbers(arr) -> number[]: Squares all numeric values in an array
- arrays/transformArrayUtils.js toStrings(arr) -> string[]: Converts all array values to strings

### Collections

- collections/arrayCollectionUtils.js chunk(arr, size) -> Array[]: Splits an array into chunks of a given size
- collections/arrayCollectionUtils.js flatten(arr) -> Array: Flattens a nested array by one level
- collections/arrayCollectionUtils.js intersection(a, b) -> Array: Returns the common elements between two arrays
- collections/arrayCollectionUtils.js unique(arr) -> Array: Removes duplicate values from an array

- collections/frequencyCollectionUtils.js countUnique(arr) -> number: Counts the number of unique items in an array
- collections/frequencyCollectionUtils.js frequency(arr) -> Object: Counts the frequency of each item in an array
- collections/frequencyCollectionUtils.js hasDuplicates(arr) -> boolean: Checks whether an array contains duplicate values
- collections/frequencyCollectionUtils.js mostFrequent(arr) -> any: Returns the most frequent item in an array

- collections/groupCollectionUtils.js filter(arr, fn) -> Array: Filters items based on a predicate function
- collections/groupCollectionUtils.js groupBy(arr, key) -> Object: Groups an array of objects by a specified key
- collections/groupCollectionUtils.js map(arr, fn) -> Array: Transforms each item using a mapping function
- collections/groupCollectionUtils.js partition(arr, fn) -> Array[]: Splits an array into two groups based on a predicate function

- collections/mapCollectionUtils.js fromMap(map) -> Object: Converts a Map into a plain object
- collections/mapCollectionUtils.js get(map, key) -> any: Retrieves a value from a Map by key
- collections/mapCollectionUtils.js set(map, key, value) -> Map: Sets a value in a Map and returns the updated Map
- collections/mapCollectionUtils.js toMap(obj) -> Map: Converts a plain object into a Map

- collections/setCollectionUtils.js contains(set, value) -> boolean: Checks whether a Set contains a value
- collections/setCollectionUtils.js fromSet(set) -> Array: Converts a Set into an array
- collections/setCollectionUtils.js toSet(arr) -> Set: Converts an array into a Set
- collections/setCollectionUtils.js union(a, b) -> Set: Computes the union of two Sets

### Conversion

- conversion/numberConversionUtils.js parseInteger(str) -> number: Parses an integer value from a string
- conversion/numberConversionUtils.js toBinary(n) -> string: Converts a number to a binary string representation
- conversion/numberConversionUtils.js toString(value) -> string: Converts a number to a string

- conversion/stringConversionUtils.js toArray(str) -> string[]: Converts a string into an array of characters 
- conversion/stringConversionUtils.js toBoolean(str) -> boolean: Converts a string value to a boolean
- conversion/stringConversionUtils.js toJSON(obj) -> string: Converts a value to a JSON string
- conversion/stringConversionUtils.js toNumber(str) -> number: Converts a string to a number

- conversion/temperatureUtils.js celsiusToFahrenheit(c) -> number: Converts Celsius to Fahrenheit
- conversion/temperatureUtils.js celsiusToKelvin(c) -> number: Converts Celsius to Kelvin
- conversion/temperatureUtils.js fahrenheitToCelsius(f) -> number: Converts Fahrenheit to Celsius
- conversion/temperatureUtils.js kelvinToCelsius(k) -> number: Converts Kelvin to Celsius 

- conversion/timeConversionUtils.js daysToHours(days) -> number: Converts days to hours
- conversion/timeConversionUtils.js hoursToMinutes(hours) -> number: Converts hours to minutes
- conversion/timeConversionUtils.js minutesToSeconds(minutes) -> number: Converts minutes to seconds
- conversion/timeConversionUtils.js secondsToMinutes(seconds) -> number: Converts seconds to minutes

### Dates

- dates/addDateUtils.js addDays(date, days) -> Date: Adds a number of days to a date
- dates/addDateUtils.js addHours(date, hours) -> Date: Adds a number of hours to a date
- dates/addDateUtils.js addMinutes(date, minutes) -> Date: Adds a number of minutes to a date
- dates/addDateUtils.js addSeconds(date, seconds) -> Date: Adds a number of seconds to a date

- dates/basicDateUtils.js getDay(date) -> number: Gets the day of the month from a date
- dates/basicDateUtils.js getMonth(date) -> number: Gets the month (0–11) from a date
- dates/basicDateUtils.js getTimestamp(date) -> number: Gets the timestamp in milliseconds for a date
- dates/basicDateUtils.js getYear(date) -> number: Gets the year from a date

- dates/compareDateUtils.js differenceInDays(date1, date2) -> number: Calculates the difference in days between two dates
- dates/compareDateUtils.js isAfter(date1, date2) -> boolean: Checks whether the first date is after the second date
- dates/compareDateUtils.js isBefore(date1, date2) -> boolean: Checks whether the first date is before the second date
- dates/compareDateUtils.js isSameDay(date1, date2) -> boolean: Checks whether two dates fall on the same day

- dates/formatDateUtils.js formatDate(date) -> string: Formats a date as YYYY-MM-DD
- dates/formatDateUtils.js formatISO(date) -> string: Formats a date as an ISO string
- dates/formatDateUtils.js formatTime(date) -> string: Formats a date as HH:MM:SS
- dates/formatDateUtils.js getWeekday(date) -> string: Returns the weekday name for a date

### Logic

- logic/booleanUtils.js and(a, b) -> boolean: Performs a logical AND operation
- logic/booleanUtils.js not(value) -> boolean: Performs a logical NOT operation
- logic/booleanUtils.js or(a, b) -> boolean: Performs a logical OR operation
- logic/booleanUtils.js xor(a, b) -> boolean: Performs a logical XOR operation

- logic/comparisonUtils.js equal(a, b) -> boolean: Checks whether two values are equal
- logic/comparisonUtils.js greaterThan(a, b) -> boolean: Checks whether a is greater than b
- logic/comparisonUtils.js lessThan(a, b) -> boolean: Checks whether a is less than b
- logic/comparisonUtils.js notEqual(a, b) -> boolean: Checks whether two values are not equal

- logic/guardUtils.js isBoolean(value) -> boolean: Checks whether a value is strictly a boolean
- logic/guardUtils.js isDefined(value) -> boolean: Checks whether a value is not null or undefined
- logic/guardUtils.js isFalsy(value) -> boolean: Checks whether a value is falsy
- logic/guardUtils.js isTruthy(value) -> boolean: Checks whether a value is truthy

- logic/rangeUtils.js between(value, min, max) -> boolean: Checks whether a value is within a range
- logic/rangeUtils.js clamp(value, min, max) -> number: Restricts a value to stay within a minimum and maximum range
- logic/rangeUtils.js randomFloat(min, max) -> number: Generates a random floating-point number within a range
- logic/rangeUtils.js randomInt(min, max) -> number: Generates a random integer within a range

- logic/truthTableUtils.js andTable() -> Array: Generates the truth table for logical AND
- logic/truthTableUtils.js orTable() -> Array: Generates the truth table for logical OR
- logic/truthTableUtils.js xorTable() -> Array: Generates the truth table for logical XOR

### Math

- math/advancedMathUtils.js absolute(n) -> number: Returns the absolute value of a number
- math/advancedMathUtils.js factorial(n) -> number: Calculates the factorial of a number
- math/advancedMathUtils.js fibonacci(n) -> number: Returns the nth Fibonacci number
- math/advancedMathUtils.js power(base, exponent) -> number: Raises a number to a given power

- math/basicMathUtils.js add(a, b) -> number: Adds two numbers
- math/basicMathUtils.js divide(a, b) -> number: Divides one number by another
- math/basicMathUtils.js multiply(a, b) -> number: Multiplies two numbers
- math/basicMathUtils.js subtract(a, b) -> number: Subtracts one number from another

- math/numberUtils.js isEven(n) -> boolean: Checks whether a number is even
- math/numberUtils.js isNegative(n) -> boolean: Checks whether a number is negative
- math/numberUtils.js isOdd(n) -> boolean: Checks whether a number is odd
- math/numberUtils.js isPositive(n) -> boolean: Checks whether a number is positive

- math/roundingUtils.js ceil(n) -> number: Rounds a number up to the nearest integer
- math/roundingUtils.js floor(n) -> number: Rounds a number down to the nearest integer
- math/roundingUtils.js roundTo(n, decimals) -> number: Rounds a number to a specified number of decimal places

- math/statisticsUtils.js average(arr) -> number: Calculates the average of an array of numbers
- math/statisticsUtils.js max(arr) -> number: Returns the maximum value in an array
- math/statisticsUtils.js min(arr) -> number: Returns the minimum value in an array
- math/statisticsUtils.js sum(arr) -> number: Calculates the sum of all values in an array

# Misc

- misc/colorUtils.js hexToRgb(hex) -> Object: Converts a HEX color string to an RGB object
- misc/colorUtils.js isHexColor(str) -> boolean: Checks whether a string is a valid HEX color
- misc/colorUtils.js randomColor() -> string: Generates a random HEX color string
- misc/colorUtils.js rgbToHex(r, g, b) -> string: Converts RGB values to a HEX color string

- misc/fileUtils.js getExtension(filename) -> string: Extracts the file extension from a filename
- misc/fileUtils.js hasExtension(filename) -> boolean: Checks whether a filename has an extension
- misc/fileUtils.js normalizeFilename(filename) -> string: Converts a filename to lowercase
- misc/fileUtils.js removeExtension(filename) -> string: Removes the file extension from a filename

- misc/formatUtils.js bytesToKB(bytes) -> number: Converts bytes to kilobytes
- misc/formatUtils.js bytesToMB(bytes) -> number: Converts bytes to megabytes
- misc/formatUtils.js label(str) -> string: Converts a string to uppercase for labeling
- misc/formatUtils.js toPercent(value) -> string: Formats a value as a percentage string

- misc/idUtils.js generateId() -> string: Generates a simple random ID
- misc/idUtils.js generateNumericId(length) -> string: Generates a numeric ID of a specified length
- misc/idUtils.js generateUUIDLike() -> string: Generates a UUID-like string
- misc/idUtils.js isValidId(str) -> boolean: Checks whether an ID string is valid

- misc/urlUtils.js getHostname(url) -> string: Extracts the hostname from a URL
- misc/urlUtils.js getPathname(url) -> string: Extracts the pathname from a URL
- misc/urlUtils.js getProtocol(url) -> string: Extracts the protocol from a URL
- misc/urlUtils.js isSecureUrl(url) -> boolean: Checks whether a URL uses a secure protocol

# Objects

- objects/basicObjectUtils.js clone(obj) -> Object: Creates a shallow copy of an object
- objects/basicObjectUtils.js entries(obj) -> Array: Returns key-value pairs of an object
- objects/basicObjectUtils.js keys(obj) -> string[]: Returns all keys of an object
- objects/basicObjectUtils.js values(obj) -> Array: Returns all values of an object

- objects/compareObjectUtils.js countKeys(obj) -> number: Counts the number of keys in an object
- objects/compareObjectUtils.js hasProperty(obj, prop) -> boolean: Checks whether an object has a given property
- objects/compareObjectUtils.js isEmptyObject(obj) -> boolean: Checks whether an object has no keys
- objects/compareObjectUtils.js shallowEqual(obj1, obj2) -> boolean: Performs a shallow equality check between two objects

- objects/mergeObjectUtils.js hasKey(obj, key) -> boolean: Checks whether an object contains a given key
- objects/mergeObjectUtils.js merge(obj1, obj2) -> Object: Merges two objects into one
- objects/mergeObjectUtils.js pick(obj, keys) -> Object: Creates a new object with only the specified keys
- objects/mergeObjectUtils.js removeKey(obj, key) -> Object: Removes a key from an object

- objects/pathObjectUtils.js exists(obj, path) -> boolean: Checks whether a given path exists in an object
- objects/pathObjectUtils.js get(obj, path) -> any: Retrieves a value from an object using a dot-separated path
- objects/pathObjectUtils.js remove(obj, path) -> Object: Removes a value from an object at a specified path
- objects/pathObjectUtils.js set(obj, path, value) -> Object: Sets a value in an object using a dot-separated path

- objects/transformObjectUtils.js fromPairs(arr) -> Object: Creates an object from an array of key-value pairs
- objects/transformObjectUtils.js invert(obj) -> Object: Swaps keys and values in an object
- objects/transformObjectUtils.js mapValues(obj, fn) -> Object: Transforms object values using a mapping function
- objects/transformObjectUtils.js toPairs(obj) -> Array: Converts an object into key-value pair entries

### Strings

- strings/caseUtils.js capitalize(str) -> string: Converts the first character of a string to uppercase
- strings/caseUtils.js lowercase(str) -> string: Converts a string to lowercase
- strings/caseUtils.js swapCase(str) -> string: Swaps the case of each character in a string
- strings/caseUtils.js uppercase(str) -> string: Converts a string to uppercase

- strings/formatUtils.js padEnd(str, length, char) -> string: Pads the end of a string to a specified length using a given character
- strings/formatUtils.js padStart(str, length, char) -> string: Pads the beginning of a string to a specified length using a given character
- strings/formatUtils.js repeat(str, times) -> string: Repeats a string a specified number of times
- strings/formatUtils.js reverseString(str) -> string: Reverses the order of characters in a string

- strings/searchUtils.js contains(str, search) -> boolean: Checks whether a string contains a search value
- strings/searchUtils.js countOccurrences(str, search) -> number: Counts occurrences of a substring in a string
- strings/searchUtils.js endsWith(str, suffix) -> boolean: Checks whether a string ends with a suffix
- strings/searchUtils.js startsWith(str, prefix) -> boolean: Checks whether a string starts with a prefix

- strings/splitUtils.js chunkString(str, size) -> string[]: Splits a string into equal-sized chunks
- strings/splitUtils.js splitByComma(str) -> string[]: Splits a string by commas into an array
- strings/splitUtils.js splitLines(str) -> string[]: Splits a string into lines
- strings/splitUtils.js splitWords(str) -> string[]: Splits a string into words based on whitespace

- strings/trimUtils.js removeExtraSpaces(str) -> string: Replaces multiple spaces with a single space and trims the string
- strings/trimUtils.js trim(str) -> string: Removes whitespace from both ends of a string
- strings/trimUtils.js trimLeft(str) -> string: Removes whitespace from the beginning of a string
- strings/trimUtils.js trimRight(str) -> string: Removes whitespace from the end of a string

### Validation

- validation/emailValidationUtils.js hasAtSymbol(str) -> boolean: Checks whether an email contains the '@' symbol
- validation/emailValidationUtils.js hasDomain(str) -> boolean: Checks whether an email contains a domain part
- validation/emailValidationUtils.js hasValidLength(str) -> boolean: Checks whether an email has a valid length
- validation/emailValidationUtils.js isEmail(str) -> boolean: Checks whether a string is a valid email format

- validation/numberValidationUtils.js inRange(value, min, max) -> boolean: Checks whether a number is within a specified range
- validation/numberValidationUtils.js isFiniteNumber(value) -> boolean: Checks whether a value is a finite number
- validation/numberValidationUtils.js isInteger(value) -> boolean: Checks whether a value is an integer
- validation/numberValidationUtils.js isNumber(value) -> boolean: Checks whether a value is a valid number

- validation/passwordValidationUtils.js hasLowercase(str) -> boolean: Checks whether a string contains lowercase letters
- validation/passwordValidationUtils.js hasMinimumLength(str, length) -> boolean: Checks whether a string meets a minimum length requirement
- validation/passwordValidationUtils.js hasNumber(str) -> boolean: Checks whether a string contains numeric characters
- validation/passwordValidationUtils.js hasUppercase(str) -> boolean: Checks whether a string contains uppercase letters

- validation/stringValidationUtils.js isAlphanumeric(str) -> boolean: Checks whether a string contains only alphanumeric characters
- validation/stringValidationUtils.js isAlphabetic(str) -> boolean: Checks whether a string contains only alphabetic characters
- validation/stringValidationUtils.js isEmptyString(str) -> boolean: Checks whether a string is empty or contains only whitespace
- validation/stringValidationUtils.js isNumeric(str) -> boolean: Checks whether a string contains only numeric characters

---
