# Sheets-Formulas

Some Fomulas I Use in Google Sheets

# Lets Say We Have A String That Has Localized Value Strings and We Need a New Column to Have 10 Percent More Than Column Called X which it Values Start from For Example Row 2 So it Will be X2 ->

```
=ARRAYFORMULA(IF(X2:X<>"", VALUE(SUBSTITUTE(X2:X, " ", "")) * 1.10, ""))
```

- Using this Formula in First Cell of a new column will result the same value but with 10 percent more. This will Remove the WhiteSpace characters and convert it to number and add 10 percent to it.
