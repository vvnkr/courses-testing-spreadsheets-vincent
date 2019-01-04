---
title: 'Template Chapter 1'
description: 'This is a template chapter.'
---

## Example exercise - What IS*() the data type?

```yaml
type: NormalExercise
key: 8253a1faa8
lang: spreadsheets
xp: 100
```

The values contained in each cell (either the things you typed, or the results of formulas) have a **data type**. Common types include number, text, date and logical.

Sometimes it is useful to check what type of data you have in each cell, since it may not be obvious just from looking at it. Google Sheets has a series of functions with names beginning "IS" that perform these checks, for example, [`ISTEXT()`](https://support.google.com/docs/answer/3093297) takes a cell address like `B3` as an input, and returns the logical value `TRUE` if the cell contains text, or `FALSE` otherwise.

Likewise, [`ISNUMBER()`](https://support.google.com/docs/answer/3093296) checks for numbers in the cell, ISDATE() checks for dates, and [`ISLOGICAL()`](https://support.google.com/docs/answer/3093351) checks for logical values.

The worksheet shows data taken from Wikipedia regarding [men's 100m sprint world records](https://en.wikipedia.org/wiki/Men%27s_100_metres_world_record_progression#Records_from_1977).

`@instructions`
Check the data types of the first row of sprint data. In cell `A21`, there is a formula to check if the value in `A2` is numeric.

- Copy the formula right as far as `G21` by dragging the bottom-right corner of `A21`.
- In cells `A22` to `G22`, check if the values in cells `A2` to `G2` are numbers by writing formulas that call `ISTEXT()`.
- In `A23` to `G23`, use `ISDATE()` to check if `A2` to `G2` are dates.
- In `A24` to `G24`, use `ISLOGICAL()` to check if `A2` to `G2` are logicals.

`@hint`
- Copy the formula in cell `A21` rightwards so that `B21` contains `=ISNUMBER(B2)`, `C21` contains `=ISNUMBER(C2)`, and so on to `F21` containing `=ISNUMBER(F2)`.
- Type `=ISTEXT(A2)` in cell `A22`, and copy rightwards to `F22` containing `=ISTEXT(F2)`.
- Below that, in cells `A23` to `F23` write `=ISDATE(A2)` to `=ISDATE(F2)`.
- Below that, repeat with `=ISLOGICAL(A2)`, etc.  
