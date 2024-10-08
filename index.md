# File: `/home/sergio/Code/helpers/src/RegExValidation.cs`

## Class: `RegExValidation`

### Method: `CheckPassword`
- **Signature**: `bool CheckPassword(string password)`
- **Description**: Checks if the given password meets the required complexity.

### Method: `IsValidEmail`
- **Signature**: `bool IsValidEmail(string email)`
- **Description**: Validates if the given string is a valid email address.

### Method: `IsValidPhoneNumber`
- **Signature**: `bool IsValidPhoneNumber(string phoneNumber)`
- **Description**: Validates if the given string is a valid phone number.

### Method: `IsValidURL`
- **Signature**: `bool IsValidURL(string url)`
- **Description**: Validates if the given string is a valid URL.

### Method: `IsValidPostalCode`
- **Signature**: `bool IsValidPostalCode(string postalCode)`
- **Description**: Validates if the given string is a valid postal code.

### Method: `IsValidCreditCard`
- **Signature**: `bool IsValidCreditCard(string creditCardNumber)`
- **Description**: Validates if the given string is a valid credit card number using the Luhn algorithm.

### Method: `IsValidIPv4`
- **Signature**: `bool IsValidIPv4(string ipAddress)`
- **Description**: Validates if the given string is a valid IPv4 address.

### Method: `IsValidIPv6`
- **Signature**: `bool IsValidIPv6(string ipAddress)`
- **Description**: Validates if the given string is a valid IPv6 address.

### Method: `IsValidSSN`
- **Signature**: `bool IsValidSSN(string ssn)`
- **Description**: Validates if the given string is a valid Social Security Number (SSN).

### Method: `IsValidUsername`
- **Signature**: `bool IsValidUsername(string username)`
- **Description**: Validates if the given string is a valid username.

### Method: `IsValidDate`
- **Signature**: `bool IsValidDate(string date, string[] dateFormats)`
- **Description**: Validates if the given date string matches any of the specified date formats.

---
# File: `/home/sergio/Code/helpers/src/BrasilDocsValidationHelper.cs`

## Class: `BrasilDocsValidationHelper`

### Method: `IsValidCEP`
- **Signature**: `bool IsValidCEP(string cep)`
- **Description**: Validates a Brazilian CEP (postal code).

### Method: `IsValidCNPJ`
- **Signature**: `bool IsValidCNPJ(string cnpj)`
- **Description**: Validates a Brazilian CNPJ (Company Identifier).

### Method: `IsValidPIS`
- **Signature**: `bool IsValidPIS(string pis)`
- **Description**: Validates a Brazilian PIS (Social Integration Program).

### Method: `IsValidCPF`
- **Signature**: `bool IsValidCPF(string cpf)`
- **Description**: Validates a Brazilian CPF (Individual Taxpayer Registry).

---
# File: `/home/sergio/Code/helpers/src/DateTimeHelper.cs`

## Class: `DateTimeHelper`

### Method: `GetFormattedDateTime`
- **Signature**: `DateTimeOffset GetFormattedDateTime(string dateTime, string dateTimeFormat)`
- **Description**: Returns a formatted DateTime (UTC) based on the provided format.

### Method: `GetAgeInYear`
- **Signature**: `double GetAgeInYear(DateTime date)`
- **Description**: Calculates the age in years from a given date.

### Method: `GetWeekNumber`
- **Signature**: `int GetWeekNumber(DateTime date)`
- **Description**: Gets the number of the week for the specified date, based on the current culture.

### Method: `GetFirstDayOfWeek`
- **Signature**: `DateTime GetFirstDayOfWeek(DateTime date)`
- **Description**: Gets the first day of the week for the given date, based on the current culture.

### Method: `GetDatesInRange`
- **Signature**: `ICollection<DateTimeOffset> GetDatesInRange(DateTimeOffset startDate, DateTimeOffset endDate, TimeSpan delta)`
- **Description**: Returns a collection of dates between the start and end date, with the specified interval.

### Method: `ConvertForTimeZone`
- **Signature**: `DateTimeOffset ConvertForTimeZone(DateTimeOffset dateTime, TimeZoneInfo timeZone)`
- **Description**: Converts the given date to the specified time zone.

### Method: `GetQuarter`
- **Signature**: `int GetQuarter(int month)`
- **Description**: Gets the quarter that corresponds to the specified month.

### Method: `GetDatesInFrequency`
- **Signature**: `IEnumerable<DateTimeOffset> GetDatesInFrequency(IEnumerable<DateTimeOffset> dates, TimeSpan frequency)`
- **Description**: Returns dates that match a given frequency within a collection.

### Method: `GetDatesEachMonth`
- **Signature**: `IEnumerable<DateTimeOffset> GetDatesEachMonth(DateTime startDate, DateTime endDate)`
- **Description**: Gets a list of dates separated by one month between the start and end date.

---
# File: `/home/sergio/Code/helpers/src/BinaryHelper.cs`

## Class: `BinaryHelper`

### Method: `ToBinary`
- **Signature**: `string ToBinary(long value)`
- **Description**: Converts a long value to a 64-bit binary string.

### Method: `ToBinary`
- **Signature**: `string ToBinary(int value)`
- **Description**: Converts an integer value to a 32-bit binary string.

### Method: `ToBinary`
- **Signature**: `string ToBinary(short value)`
- **Description**: Converts a short value to a 16-bit binary string.

### Method: `GetBitValue`
- **Signature**: `bool GetBitValue(long value, int position)`
- **Description**: Gets the boolean value from a specific bit position in a long value using bitwise operations.

### Method: `GetBitValue`
- **Signature**: `bool GetBitValue(int value, int position)`
- **Description**: Gets the boolean value from a specific bit position in an integer value using bitwise operations.

### Method: `GetBitValue`
- **Signature**: `bool GetBitValue(short value, int position)`
- **Description**: Gets the boolean value from a specific bit position in a short value using bitwise operations.

### Method: `GetBitsValue`
- **Signature**: `int GetBitsValue(long value, int startBitPosition, int endBitPosition)`
- **Description**: Gets the integer value from a specific bit range in a long value.

### Method: `SetBitValue`
- **Signature**: `long SetBitValue(long value, int position, bool bitValue)`
- **Description**: Sets a specific bit in a long value to 1 or 0.

### Method: `ToggleBitValue`
- **Signature**: `long ToggleBitValue(long value, int position)`
- **Description**: Toggles a specific bit in a long value.

---
# File: `/home/sergio/Code/helpers/src/SSLHelper.cs`

## Class: `SslHelper`

### Method: `IgnoreCertificateWarning`
- **Signature**: `void IgnoreCertificateWarning()`
- **Description**: Ignores all SSL certificate warnings. Use only for development purposes.

### Method: `RestoreCertificateValidation`
- **Signature**: `void RestoreCertificateValidation()`
- **Description**: Restores the default SSL certificate validation behavior.

### Method: `SetCustomCertificateValidation`
- **Signature**: `void SetCustomCertificateValidation(RemoteCertificateValidationCallback validationCallback)`
- **Description**: Sets a custom SSL certificate validation callback.

### Method: `IgnoreCertificateWarningTemporarily`
- **Signature**: `void IgnoreCertificateWarningTemporarily(Action action)`
- **Description**: Temporarily ignores SSL certificate warnings for a specific action.

---
# File: `/home/sergio/Code/helpers/src/UriHelper.cs`

## Class: `UriHelper`

### Method: `GetUri`
- **Signature**: `Uri GetUri(Uri uri, string ip, string port)`
- **Description**: Constructs a new URI using the specified IP and port, retaining the scheme and local path of the original URI.

### Method: `AddOrUpdateQueryParam`
- **Signature**: `Uri AddOrUpdateQueryParam(Uri uri, string paramName, string paramValue)`
- **Description**: Adds or updates a query parameter in the URI.

### Method: `RemoveQueryParam`
- **Signature**: `Uri RemoveQueryParam(Uri uri, string paramName)`
- **Description**: Removes a query parameter from the URI.

### Method: `IsValidUri`
- **Signature**: `bool IsValidUri(string uri)`
- **Description**: Checks if a URI is valid.

### Method: `GetHostAndPort`
- **Signature**: `(string Host, int Port) GetHostAndPort(Uri uri)`
- **Description**: Gets the host and port from the URI.

### Method: `BuildUri`
- **Signature**: `Uri BuildUri(string scheme, string host, int port, string path, IDictionary<string, string> queryParams)`
- **Description**: Builds a URI from separate parts.

---
# File: `/home/sergio/Code/helpers/src/StringHelper.cs`

## Class: `StringHelper`

### Method: `IsAlpha`
- **Signature**: `bool IsAlpha(string strToCheck)`
- **Description**: Checks if the string contains only alphabetic characters.

### Method: `IsAlphaNumeric`
- **Signature**: `bool IsAlphaNumeric(string strToCheck)`
- **Description**: Checks if the string contains only alphanumeric characters.

### Method: `ToDoubleNullable`
- **Signature**: `double? ToDoubleNullable(string value)`
- **Description**: Converts the string to a double if the value is numeric. If not numeric, returns NULL.

### Method: `ToEnumerable`
- **Signature**: `IEnumerable<string> ToEnumerable(string text)`
- **Description**: Fills an IEnumerable with each line of a string.

### Method: `TextAfter`
- **Signature**: `string? TextAfter(string value, string search)`
- **Description**: Extracts a substring right after a given string.

### Method: `GetTextFromLine`
- **Signature**: `string? GetTextFromLine(string text, int lineNo)`
- **Description**: Gets a text from a specific line in a string.

### Method: `GetLineNumber`
- **Signature**: `int GetLineNumber(string text, string lineToFind)`
- **Description**: Gets the line position of a substring in a given text.

### Method: `IsNumeric`
- **Signature**: `bool IsNumeric(string strToCheck)`
- **Description**: Checks if the string contains only numeric characters.

### Method: `ToTitleCase`
- **Signature**: `string ToTitleCase(string str)`
- **Description**: Converts the string to title case (capitalizes the first letter of each word).

### Method: `ReverseString`
- **Signature**: `string ReverseString(string str)`
- **Description**: Reverses the characters in the string.

### Method: `IsInteger`
- **Signature**: `bool IsInteger(string strToCheck)`
- **Description**: Checks if the string is a valid integer.

### Method: `IsValidDate`
- **Signature**: `bool IsValidDate(string strToCheck, string dateFormat)`
- **Description**: Checks if the string is a valid date.

### Method: `HasData`
- **Signature**: `bool HasData(string value)`
- **Description**: Extension method to check if a string is not null or empty.

### Method: `RemoveExtraSpaces`
- **Signature**: `string RemoveExtraSpaces(string str)`
- **Description**: Removes extra white spaces from the string.

### Method: `IsValidEmail`
- **Signature**: `bool IsValidEmail(string email)`
- **Description**: Checks if the string is a valid email address.

### Method: `IsValidUrl`
- **Signature**: `bool IsValidUrl(string url)`
- **Description**: Checks if the string is a valid URL.

### Method: `Truncate`
- **Signature**: `string Truncate(string str, int maxLength)`
- **Description**: Truncates the string to the specified length.

### Method: `ReplaceMultipleSpaces`
- **Signature**: `string ReplaceMultipleSpaces(string str)`
- **Description**: Replaces multiple spaces in the string with a single space.

### Method: `RemoveNonAlphanumeric`
- **Signature**: `string RemoveNonAlphanumeric(string str)`
- **Description**: Removes non-alphanumeric characters from the string.

### Method: `ToCamelCase`
- **Signature**: `string ToCamelCase(string str)`
- **Description**: Converts the string to camelCase.

### Method: `ToSnakeCase`
- **Signature**: `string ToSnakeCase(string str)`
- **Description**: Converts the string to snake_case.

---
# File: `/home/sergio/Code/helpers/src/BooleanHelper.cs`

## Class: `BooleanHelper`

### Method: `GetBooleanIntValueFromString`
- **Signature**: `int GetBooleanIntValueFromString(string value)`
- **Description**: Converts a string value to an integer representation of a boolean (1 for true, 0 for false). Throws an exception if the value cannot be parsed.

### Method: `TryParseBooleanIntValueFromString`
- **Signature**: `bool TryParseBooleanIntValueFromString(string value, int boolValue)`
- **Description**: Attempts to parse a string value into an integer representation of a boolean (1 for true, 0 for false).

### Method: `GetBooleanFromString`
- **Signature**: `bool GetBooleanFromString(string value)`
- **Description**: Converts a string value to a boolean. Throws an exception if the value cannot be parsed.

### Method: `TryParseBooleanFromString`
- **Signature**: `bool TryParseBooleanFromString(string value, bool boolValue)`
- **Description**: Attempts to parse a string value into a boolean.

### Method: `GetBooleanFromString`
- **Signature**: `bool GetBooleanFromString(string value, string trueString, string falseString)`
- **Description**: Converts a string value to a boolean based on custom true/false string representations. Throws an exception if the value cannot be parsed.

### Method: `TryParseBooleanFromString`
- **Signature**: `bool TryParseBooleanFromString(string value, string trueString, string falseString, bool boolValue)`
- **Description**: Attempts to parse a string value into a boolean based on custom true/false string representations.

### Method: `FormatBooleanToString`
- **Signature**: `string FormatBooleanToString(bool value, string trueString, string falseString)`
- **Description**: Formats a boolean value to a string representation based on input parameters.

---
# File: `/home/sergio/Code/helpers/src/NetworkHelper.cs`

## Class: `NetworkHelper`

### Method: `GetLocalIpAddress`
- **Signature**: `string GetLocalIpAddress()`
- **Description**: Gets the primary local IPv4 address.

### Method: `GetAllLocalIpAddresses`
- **Signature**: `IEnumerable<string> GetAllLocalIpAddresses()`
- **Description**: Gets all local IPv4 addresses.

### Method: `IsPortOpen`
- **Signature**: `bool IsPortOpen(string host, int port, TimeSpan timeout)`
- **Description**: Checks if the specified port is open on the given host.

### Method: `PingHost`
- **Signature**: `bool PingHost(string host)`
- **Description**: Pings the specified host synchronously.

### Method: `PingHostAsync`
- **Signature**: `Task<bool> PingHostAsync(string host)`
- **Description**: Pings the specified host asynchronously.

### Method: `GetMacAddress`
- **Signature**: `string GetMacAddress()`
- **Description**: Gets the MAC address of the first network adapter.

### Method: `GetNetworkInterfaces`
- **Signature**: `IEnumerable<NetworkInterface> GetNetworkInterfaces()`
- **Description**: Gets all network interfaces on the local machine.

### Method: `IsValidIpAddress`
- **Signature**: `bool IsValidIpAddress(string ipAddress)`
- **Description**: Checks if the provided string is a valid IPv4 or IPv6 address.

### Method: `IsUrlReachableAsync`
- **Signature**: `Task<bool> IsUrlReachableAsync(string url)`
- **Description**: Checks if the specified URL is reachable.

### Method: `IsInternetAvailable`
- **Signature**: `bool IsInternetAvailable()`
- **Description**: Checks if the internet is available by pinging an external IP (e.g., Google's public DNS).

### Method: `GetAvailablePort`
- **Signature**: `int GetAvailablePort()`
- **Description**: Gets an available port on the local machine.

---
# File: `/home/sergio/Code/helpers/src/EnumerableExtensions.cs`

## Class: `EnumerableExtensions`

### Method: `HasData`
- **Signature**: `bool HasData(IEnumerable<T>? list)`
- **Description**: Checks if a collection is not null and is not empty.

### Method: `IndexOf`
- **Signature**: `int IndexOf(IList<T> obj, T value)`
- **Description**: Finds the index of a value in a list using a default equality comparer.

### Method: `IndexOf`
- **Signature**: `int IndexOf(IEnumerable<T> obj, T value, IEqualityComparer<T> comparer)`
- **Description**: Finds the index of a value in an enumerable collection using a specified comparer.

### Method: `FindItemWithNeighbors`
- **Signature**: `(T? Previous, T? Current, T? Next) FindItemWithNeighbors(IEnumerable<T> items, Predicate<T> matchFilling)`
- **Description**: Finds the item in the collection that is sandwiched between two other items.

### Method: `IsEmpty`
- **Signature**: `bool IsEmpty(IEnumerable<T> source)`
- **Description**: Checks if the collection is empty.

### Method: `ForEach`
- **Signature**: `void ForEach(IEnumerable<T> source, Action<T> action)`
- **Description**: Performs the specified action on each element of the collection.

### Method: `ToCommaSeparatedString`
- **Signature**: `string ToCommaSeparatedString(IEnumerable<T> source)`
- **Description**: Converts the collection to a comma-separated string.

### Method: `ChunkBy`
- **Signature**: `IEnumerable<IEnumerable<T>> ChunkBy(IEnumerable<T> source, int size)`
- **Description**: Splits the collection into chunks of the specified size.

### Method: `DistinctBy`
- **Signature**: `IEnumerable<TSource> DistinctBy(IEnumerable<TSource> source, Func<TSource, TKey> keySelector)`
- **Description**: Returns distinct elements from a sequence by using a specified selector.

### Method: `Shuffle`
- **Signature**: `IEnumerable<T> Shuffle(IEnumerable<T> source)`
- **Description**: Shuffles the elements of the collection randomly.

### Method: `Partition`
- **Signature**: `(IEnumerable<T> Matches, IEnumerable<T> NonMatches) Partition(IEnumerable<T> source, Func<T, bool> predicate)`
- **Description**: Partitions a collection into two collections based on a predicate.

---
# File: `/home/sergio/Code/helpers/src/SerializationHelper.cs`

## Class: `SerializationHelper`

### Method: `SerializeToXml`
- **Signature**: `XmlDocument SerializeToXml(T obj)`
- **Description**: Serializes an object to an XmlDocument.

### Method: `DeserializeFromXml`
- **Signature**: `T DeserializeFromXml(XmlReader xml)`
- **Description**: Deserializes an object from an XmlReader.

### Method: `SerializeDataContract`
- **Signature**: `string SerializeDataContract(T obj)`
- **Description**: Serializes an object to a string using DataContractSerializer.

### Method: `DeserializeDataContract`
- **Signature**: `T DeserializeDataContract(string data)`
- **Description**: Deserializes an object from a string using DataContractSerializer.

### Method: `SerializeToJson`
- **Signature**: `string SerializeToJson(T obj)`
- **Description**: Serializes an object to a JSON string using System.Text.Json.

### Method: `DeserializeFromJson`
- **Signature**: `T DeserializeFromJson(string json)`
- **Description**: Deserializes an object from a JSON string using System.Text.Json.

### Method: `IsValidXml`
- **Signature**: `bool IsValidXml(string xml)`
- **Description**: Validates if a string is a well-formed XML.

### Method: `IsValidJson`
- **Signature**: `bool IsValidJson(string json)`
- **Description**: Validates if a string is a well-formed JSON.

### Method: `FormatXml`
- **Signature**: `string FormatXml(XmlDocument xmlDoc)`
- **Description**: Formats an XmlDocument to a pretty-printed string.

### Method: `Compress`
- **Signature**: `byte[] Compress(T obj)`
- **Description**: Compresses an object to a byte array using GZip.

### Method: `Decompress`
- **Signature**: `T Decompress(byte[] compressedData)`
- **Description**: Decompresses an object from a byte array using GZip.

### Method: `SerializeToBinary`
- **Signature**: `byte[] SerializeToBinary(T obj)`
- **Description**: Serializes an object to a byte array using BinaryFormatter.

### Method: `SerializeToJsonByteArray`
- **Signature**: `byte[] SerializeToJsonByteArray(T obj)`
- **Description**: Serializes an object to a byte array using JSON serialization.

### Method: `DeserializeFromBinary`
- **Signature**: `T DeserializeFromBinary(byte[] data)`
- **Description**: Deserializes an object from a byte array using BinaryFormatter.

### Method: `DeserializeFromJsonByteArray`
- **Signature**: `T DeserializeFromJsonByteArray(byte[] data)`
- **Description**: Deserializes an object of type <typeparamref name="T"/> from a JSON byte array.

---
# File: `/home/sergio/Code/helpers/src/NameOfHelper.cs`

## Class: `NameOfHelper`

### Method: `GetPropertyName`
- **Signature**: `string GetPropertyName(T obj, Expression<Func<T, TProp>> propertyAccessor)`
- **Description**: Gets the name of a property from a given lambda expression.

---
# File: `/home/sergio/Code/helpers/src/UnitHelper.cs`

## Class: `UnitHelper`

### Method: `ConvertDegreeToKelvin`
- **Signature**: `double ConvertDegreeToKelvin(double value)`
- **Description**: Converts degrees Celsius to Kelvin.

### Method: `ConvertKelvinToDegree`
- **Signature**: `double ConvertKelvinToDegree(double value)`
- **Description**: Converts Kelvin to degrees Celsius.

### Method: `ConvertCelsiusToFahrenheit`
- **Signature**: `double ConvertCelsiusToFahrenheit(double value)`
- **Description**: Converts degrees Celsius to degrees Fahrenheit.

### Method: `ConvertFahrenheitToCelsius`
- **Signature**: `double ConvertFahrenheitToCelsius(double value)`
- **Description**: Converts degrees Fahrenheit to degrees Celsius.

### Method: `ConvertMilesToKilometers`
- **Signature**: `double ConvertMilesToKilometers(double value)`
- **Description**: Converts miles to kilometers.

### Method: `ConvertKilometersToMiles`
- **Signature**: `double ConvertKilometersToMiles(double value)`
- **Description**: Converts kilometers to miles.

### Method: `ConvertPoundsToKilograms`
- **Signature**: `double ConvertPoundsToKilograms(double value)`
- **Description**: Converts pounds to kilograms.

### Method: `ConvertKilogramsToPounds`
- **Signature**: `double ConvertKilogramsToPounds(double value)`
- **Description**: Converts kilograms to pounds.

### Method: `ConvertLitersToGallons`
- **Signature**: `double ConvertLitersToGallons(double value)`
- **Description**: Converts liters to gallons.

### Method: `ConvertGallonsToLiters`
- **Signature**: `double ConvertGallonsToLiters(double value)`
- **Description**: Converts gallons to liters.

### Method: `ConvertInchesToCentimeters`
- **Signature**: `double ConvertInchesToCentimeters(double value)`
- **Description**: Converts inches to centimeters.

### Method: `ConvertCentimetersToInches`
- **Signature**: `double ConvertCentimetersToInches(double value)`
- **Description**: Converts centimeters to inches.

---
# File: `/home/sergio/Code/helpers/src/FloatingNumberHelper.cs`

## Class: `FloatingNumberHelper`

### Method: `NearlyEqual`
- **Signature**: `bool NearlyEqual(double value, double compareTo, double epsilon)`
- **Description**: Checks if two double values are nearly equal, allowing for a specified tolerance.

### Method: `NearlyEqual`
- **Signature**: `bool NearlyEqual(double value, double compareTo)`
- **Description**: Checks if two double values are nearly equal, using the default tolerance.

### Method: `NearlyEqual`
- **Signature**: `bool NearlyEqual(double? value, double? compareTo)`
- **Description**: Checks if two nullable double values are nearly equal, allowing for default tolerance.

### Method: `NearlyEqual`
- **Signature**: `bool NearlyEqual(double value, double? compareTo)`
- **Description**: Checks if a double value is nearly equal to a nullable double value, using the default tolerance.

### Method: `NearlyZero`
- **Signature**: `bool NearlyZero(double value, double epsilon)`
- **Description**: Checks if a double value is nearly zero, allowing for a specified tolerance.

### Method: `NearlyZero`
- **Signature**: `bool NearlyZero(double value)`
- **Description**: Checks if a double value is nearly zero, using the default tolerance.

### Method: `NearlyZero`
- **Signature**: `bool NearlyZero(double? value)`
- **Description**: Checks if a nullable double value is nearly zero, using the default tolerance.

### Method: `NearlyZeroOrNull`
- **Signature**: `bool NearlyZeroOrNull(double? value)`
- **Description**: Checks if a nullable double value is nearly zero or null, using the default tolerance.

### Method: `NearlyZero`
- **Signature**: `bool NearlyZero(float value, float epsilon)`
- **Description**: Checks if a float value is nearly zero, allowing for a specified tolerance.

### Method: `NearlyZero`
- **Signature**: `bool NearlyZero(float value)`
- **Description**: Checks if a float value is nearly zero, using the default tolerance.

### Method: `NearlyEqual`
- **Signature**: `bool NearlyEqual(float value, float compareTo)`
- **Description**: Checks if two float values are nearly equal, using the default tolerance.

### Method: `GreaterThanOrNearlyEqual`
- **Signature**: `bool GreaterThanOrNearlyEqual(double value, double compareTo)`
- **Description**: Checks if a double value is greater than or nearly equal to another value, allowing for the default tolerance.

### Method: `LessThanOrNearlyEqual`
- **Signature**: `bool LessThanOrNearlyEqual(double value, double compareTo)`
- **Description**: Checks if a double value is less than or nearly equal to another value, allowing for the default tolerance.

---
# File: `/home/sergio/Code/helpers/src/NumericHelper.cs`

## Class: `NumericHelper`

### Method: `GetDoubleFromString`
- **Signature**: `double GetDoubleFromString(string value)`
- **Description**: Converts a string to a double value.

### Method: `TryGetDoubleFromString`
- **Signature**: `bool TryGetDoubleFromString(string value, double doubleValue)`
- **Description**: Attempts to convert a string to a double value.

### Method: `GetFloatFromString`
- **Signature**: `float GetFloatFromString(string value)`
- **Description**: Converts a string to a float value.

### Method: `GetIntFromString`
- **Signature**: `int GetIntFromString(string value)`
- **Description**: Converts a string to an integer value.

### Method: `TryGetIntFromString`
- **Signature**: `bool TryGetIntFromString(string value, int intValue)`
- **Description**: Attempts to convert a string to an integer value.

### Method: `GetDecimalFromString`
- **Signature**: `decimal GetDecimalFromString(string value)`
- **Description**: Converts a string to a decimal value.

### Method: `Truncate`
- **Signature**: `double Truncate(double value, int precision)`
- **Description**: Truncates a double value to a specified number of decimal places.

### Method: `IsValidNumericValue`
- **Signature**: `bool IsValidNumericValue(double value)`
- **Description**: Checks if the numeric value is valid (not NaN or infinity).

### Method: `IsNaturalNumber`
- **Signature**: `bool IsNaturalNumber(string strNumber)`
- **Description**: Checks if the string represents a natural number (positive and without fractions).

### Method: `IsWholeNumber`
- **Signature**: `bool IsWholeNumber(string strNumber)`
- **Description**: Checks if the string represents a non-negative integer.

### Method: `IsInteger`
- **Signature**: `bool IsInteger(string strNumber)`
- **Description**: Checks if the string represents an integer (positive or negative).

### Method: `IsPositiveNumber`
- **Signature**: `bool IsPositiveNumber(string strNumber)`
- **Description**: Checks if the string represents a positive number (integer or real).

### Method: `IsNumber`
- **Signature**: `bool IsNumber(string strNumber)`
- **Description**: Checks if the string represents a valid number.

### Method: `IsInRange`
- **Signature**: `bool IsInRange(double value, double min, double max)`
- **Description**: Checks if a value is within a specific range.

### Method: `GetDoubleOrDefault`
- **Signature**: `double GetDoubleOrDefault(string value, double defaultValue)`
- **Description**: Attempts to get a double value from a string, returning a default value if it fails.

### Method: `ToCurrency`
- **Signature**: `string ToCurrency(double value, string culture)`
- **Description**: Converts a double value to a currency representation in a specific culture.

---
# File: `/home/sergio/Code/helpers/src/FileHelper.cs`

## Class: `FileHelper`

### Method: `RemoveIllegalFileNameChars`
- **Signature**: `string RemoveIllegalFileNameChars(string input, string replacement)`
- **Description**: Removes illegal characters from a file name or path.

### Method: `ReadAllLines`
- **Signature**: `string[] ReadAllLines(string filePath)`
- **Description**: Reads all lines from a text file.

### Method: `WriteAllLines`
- **Signature**: `void WriteAllLines(string filePath, string[] lines)`
- **Description**: Writes all lines to a text file.

### Method: `ReadAllText`
- **Signature**: `string ReadAllText(string filePath)`
- **Description**: Reads all text from a file.

### Method: `WriteAllText`
- **Signature**: `void WriteAllText(string filePath, string text)`
- **Description**: Writes text to a file.

### Method: `AppendAllText`
- **Signature**: `void AppendAllText(string filePath, string text)`
- **Description**: Appends text to a file, creating the file if it does not exist.

### Method: `FileExists`
- **Signature**: `bool FileExists(string filePath)`
- **Description**: Checks if a file exists.

### Method: `DeleteFile`
- **Signature**: `void DeleteFile(string filePath)`
- **Description**: Deletes a file.

### Method: `CopyFile`
- **Signature**: `void CopyFile(string sourceFilePath, string destFilePath, bool overwrite)`
- **Description**: Copies a file to a new location.

### Method: `MoveFile`
- **Signature**: `void MoveFile(string sourceFilePath, string destFilePath)`
- **Description**: Moves a file to a new location.

## Class: `FileExtensionMethods`

### Method: `ToFileSize`
- **Signature**: `string ToFileSize(long l)`
- **Description**: Converts a long value representing bytes into a formatted file size string.

## Class: `FileSizeFormatProvider`

### Method: `GetFormat`
- **Signature**: `object? GetFormat(Type? formatType)`
- **Description**: No summary available.

### Method: `Format`
- **Signature**: `string Format(string? format, object? arg, IFormatProvider? formatProvider)`
- **Description**: No summary available.

---
# File: `/home/sergio/Code/helpers/src/TreeHelper.cs`

## Class: `TreeHelper`

### Method: `GetAllNodes`
- **Signature**: `IEnumerable<T> GetAllNodes(T treeNode, Func<T,IEnumerable<T>> getChildren)`
- **Description**: Return all nodes in a list

### Method: `DoActionOnCondition`
- **Signature**: `void DoActionOnCondition(T treeNode, Func<T,IEnumerable<T>> getChildren, Func<T, bool> condition, Action<T> action, Action<T>? elseAction)`
- **Description**: Do the action on each node if matching to the condition

### Method: `GetTree`
- **Signature**: `T? GetTree(P rootId, IEnumerable<T> items, Func<T, P> id, Func<T, P?> parentId, Func<T, IList<T>> children)`
- **Description**: Get site tree

---
# File: `/home/sergio/Code/helpers/src/EnumHelper.cs`

## Class: `EnumHelper`

### Method: `GetList`
- **Signature**: `IEnumerable<T> GetList()`
- **Description**: Gets a list of all values in the enum.

### Method: `Parse`
- **Signature**: `T Parse(int value)`
- **Description**: Parses an integer value to the corresponding enum value.

### Method: `Parse`
- **Signature**: `T Parse(string value)`
- **Description**: Parses a string value to the corresponding enum value.

### Method: `TryParse`
- **Signature**: `bool TryParse(int value, T enumValue)`
- **Description**: Attempts to parse an integer value to the corresponding enum value.

### Method: `TryParse`
- **Signature**: `bool TryParse(string value, T enumValue)`
- **Description**: Attempts to parse a string value to the corresponding enum value.

### Method: `GetAttributeOfType`
- **Signature**: `T? GetAttributeOfType(Enum enumVal)`
- **Description**: Gets the attribute of a specified type associated with an enum value.

### Method: `GetDescription`
- **Signature**: `string GetDescription(Enum enumVal)`
- **Description**: Gets the description attribute of an enum value.

### Method: `ToList`
- **Signature**: `List<KeyValuePair<string, int>> ToList()`
- **Description**: Converts the enum values to a list of their names and integer values.

### Method: `IsDefined`
- **Signature**: `bool IsDefined(int value)`
- **Description**: Checks if an integer value is defined in the specified enum.

### Method: `IsDefined`
- **Signature**: `bool IsDefined(string value)`
- **Description**: Checks if a string value is defined in the specified enum.

### Method: `GetNames`
- **Signature**: `List<string> GetNames()`
- **Description**: Gets the names of the enum values as a list of strings.

### Method: `GetValues`
- **Signature**: `List<int> GetValues()`
- **Description**: Gets the values of the enum as a list of integers.

### Method: `GetDefaultValue`
- **Signature**: `T GetDefaultValue()`
- **Description**: Gets the default value of the specified enum type.

### Method: `ConvertToDescriptionDictionary`
- **Signature**: `Dictionary<int, string> ConvertToDescriptionDictionary()`
- **Description**: Converts the enum values to a dictionary of their integer values and descriptions.

---
# File: `/home/sergio/Code/helpers/src/MathHelper.cs`

## Class: `MathHelper`

### Method: `GetLeastSquaresTrend`
- **Signature**: `double GetLeastSquaresTrend(IList<Tuple<float, float>> serie)`
- **Description**: Computes the trend of a series using the Least Squares method.

### Method: `GetMinMaxAvg`
- **Signature**: `void GetMinMaxAvg(IList<double> serie, double min, double max, double avg)`
- **Description**: Computes the minimum, maximum, and average of a series of values.

### Method: `GetDiscrepancy`
- **Signature**: `double GetDiscrepancy(IEnumerable<double> values)`
- **Description**: Returns the discrepancy between the maximum and minimum values in the series.

### Method: `CalculateStandardDeviation`
- **Signature**: `void CalculateStandardDeviation(IEnumerable<double> values, double? average, double? stdDeviation)`
- **Description**: Computes the standard deviation of a series.

### Method: `GetAverage`
- **Signature**: `double? GetAverage(IList<KeyValuePair<DateTimeOffset, double>> values)`
- **Description**: Computes the weighted average of a series of values with associated timestamps.

### Method: `GetAverageSquare`
- **Signature**: `double? GetAverageSquare(IList<KeyValuePair<DateTimeOffset, double>> values)`
- **Description**: Computes the average squared value of a series of values with associated timestamps.

### Method: `GetStandardDeviation`
- **Signature**: `double? GetStandardDeviation(IList<KeyValuePair<DateTimeOffset, double>> values, double average)`
- **Description**: Computes the standard deviation of a series using its average and squared average.

---
# File: `/home/sergio/Code/helpers/src/TimeseriesHelper.cs`

## Class: `TimeseriesHelper`

### Method: `GetPeriodeSpansUnderThreshold`
- **Signature**: `IEnumerable<Tuple<DateTimeOffset, DateTimeOffset>> GetPeriodeSpansUnderThreshold(IEnumerable<KeyValuePair<DateTimeOffset, double>> timeseriesValues, double threshold)`
- **Description**: Return period under threshold

### Method: `ExcludeSpan`
- **Signature**: `IEnumerable<KeyValuePair<DateTimeOffset, double>> ExcludeSpan(IEnumerable<KeyValuePair<DateTimeOffset, double>> timeseriesValues, IEnumerable<Tuple<DateTimeOffset, DateTimeOffset>> spansToExclude)`
- **Description**: Exclude from timeseries values the date periode passed in parameter

---
# File: `/home/sergio/Code/helpers/src/Base64Helper.cs`

## Class: `Base64Helper`

### Method: `SafeConvertFromBase64String`
- **Signature**: `byte[] SafeConvertFromBase64String(string? input)`
- **Description**: Safely decodes a Base64-encoded string into a byte array. <para> The method replaces URL-safe characters ('-' and '_') with the standard Base64 characters ('+' and '/'). It then ensures that the string length is a multiple of 4 by appending '=' padding characters as necessary. </para> <para> If the input string is null, empty, or consists only of white spaces, the method returns an empty byte array. In case of any errors during the decoding process (e.g., if the input is not valid Base64), the method also returns an empty byte array. </para>

### Method: `EncodeToBase64String`
- **Signature**: `string EncodeToBase64String(byte[]? input)`
- **Description**: Encodes a byte array into a Base64-encoded string.

### Method: `ConvertFromBase64String`
- **Signature**: `byte[] ConvertFromBase64String(string? input, bool throwOnInvalidInput)`
- **Description**: Decodes a Base64-encoded string into a byte array with an option to throw an exception if the input is invalid.

---
# File: `/home/sergio/Code/helpers/src/StreamHelper.cs`

## Class: `StreamHelper`

### Method: `CopyStream`
- **Signature**: `void CopyStream(Stream input, Stream output)`
- **Description**: Copies the contents of input to output. Doesn't close either stream.

---
