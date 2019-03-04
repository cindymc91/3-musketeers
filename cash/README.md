# cash

> A simple module to help you convert amount of money, from one currency to another

#Usage

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
(All the available currencies are given in `cash/lib/currencies.json`)
`node bin/index.js 10 USD EUR` will convert 10 `USD` in `EUR`

```
✔ 8.821 (EUR) Euro

Conversion of USD 10
```

`node bin/index.js 10 EUR CNY` will convert 10 `EUR` in `CNY` (Chinese Yuan)

```
✔ 75.985 (CNY) Chinese Yuan

Conversion of EUR 10
```









---
