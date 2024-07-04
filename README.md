# iso-country-validator
Includes a complete list of countries and country name validation based on ISO standards.

## Installation

Install the package using npm:

```bash
npm install iso-country-validator
```

## Usage

### Listing Countries

You can list all available countries using the `countryList()` function:

```javascript

countries = require('iso-country-validator')
const getCountries = countries.countryList();
console.log(getCountries);

// Output: [{ name: [ 'Afghanistan', 'AF', 'AFG' ] }, { name: [ 'Albania', 'AL', 'ALB' ] }, ...]

```

### Validating Country Names

You can validate if a given string is a valid country name using the `checkCountryValidity()` function:

```javascript
const countries = require('iso-country-validator');

console.log(countries.checkCountryValidity('nigeria')); // true
console.log(isValidCountryName('Nigeria')); // true
console.log(isValidCountryName('NG')); // true
console.log(isValidCountryName('narnia')); // false
```
The input is not case sensitive and would work irrespective of whether the letters are in capital or not.

## API

### `countryList()`

Returns an array of all country names.

### `checkCountryValidity(name)`

- `name` (String): The country name to validate.
- Returns `true` if `name` is a valid country name, otherwise `false`.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests for any improvements or bug fixes.

1. Fork the repository at https://github.com/Lonercode/iso-country-validator.git
2. Create your feature branch (`git checkout -b feature/awesome-feature`).
3. Commit your changes (`git commit -am 'Add awesome feature'`).
4. Push to the branch (`git push origin feature/awesome-feature`).
5. Open a pull request.

