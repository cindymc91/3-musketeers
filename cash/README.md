# Cash

> A simple module to help you convert amount of money, from one currency to another

# Usage

> How the module works : currency converter

You can use the converter module by applying the following steps :
1. Open a command line shell
2. Go to the cash module folder `cd yourpath/3-musketeers/cash`
3. Execute the `index.js` file : `node bin/index.js`

At this point, the default configuration is to convert `1 USD` to 3 other currencies : `EUR`, `GBP`, `JPY`. <br>
It should output this :

```
✔ 0.882 (EUR) Euro
✔ 0.757 (GBP) British Pound Sterling
✔ 111.943 (JPY) Japanese Yen

Conversion of USD 1
```

It is possible to choose the amount to convert with `node bin/index.js <amount>` : <br>
`node bin/index.js 10` will convert 10 `USD` in `EUR`, `GBP`, `JPY`

```
✔ 8.821 (EUR) Euro
✔ 7.566 (GBP) British Pound Sterling
✔ 1119.432 (JPY) Japanese Yen

Conversion of USD 10
```

It is even possible to choose the currency you want with `node bin/index.js <amount> <from> <to>` : <br>
(All the available currencies are given in `cash/lib/currencies.json`) <br>
`node bin/index.js 10 USD EUR` will convert 10 `USD` in `EUR` :

```
✔ 8.821 (EUR) Euro

Conversion of USD 10
```

`node bin/index.js 10 EUR CNY` will convert 10 `EUR` in `CNY` (Chinese Yuan) :

```
✔ 75.985 (CNY) Chinese Yuan

Conversion of EUR 10
```

# API

> Anyone can use this module, it includes itself very smoothly in your project

To use the `cash` module, just add this line at the top of your project :

```js
const cash = require('./cash.js');
```

Then, define a constant with the following information :
- `amount`(int, float) - the amount of money you want to convert
- `from` (string) - initial currency
- `to` ([string]) - final currency

```js
const command = {
	amount: 10,
	from: USD,
	to: EUR
};

cash(command);
```

# Installation

> Now let's get into it

To use the cash module, apply the following steps : <br>
1. Fork the project from Github `https://github.com/cindymc91/3-musketeers.git`
2. Go to the location of your project and to the module `cd yourpath/3-musketeers/cash`
3. Execute the installation of every needed packages : `npm i`
4. You are ready to include this module to your own project

# License



















---
