---
title: 'Introduction to R for Finance'
output: html_document
description: 'Chapter 1'
---

## Basic Calculator

```yaml
type: BlanksChallenge
key: e1b207d0ed
```

`@context`


`@code1`
```{r}
{{var1}} <- {{var2}} {{_fun1}} {{var3}}{{_fun2}}{{var4}}
{{var1}}
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
  - 'x'
  - 'y'
  - 'z'
var2:
  - '8'
  - '4'
var3:
  - '3'
  - '2'
var4:
  - '2'
  - '3'
fun1:
  - '+'
fun2:
  - '**'
```

`@distractors`
```yaml
fun1:
 - '-'
 - '/'
 - '%'
fun2:
 - '*'
 - '+'
 - '%%'
```

---

## Basic Assignment

```yaml
type: BlanksChallenge
key: 2fbaa56717
```

`@context`


`@code1`
```{r}
{{var1}} {{_var2}} {{var3}} * {{var4}} * {{var4}}
{{var1}}
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
  - 'a'
  - 'b'
  - 'c'
var2:
  - '<-'
var3:
  - '100'
  - '75'
  - '50'
var4:
  - '1.02'
  - '1.05'
  - '1.075'
```

`@distractors`
```yaml
var2:
  - '<'
  - '<<'
  - '-'
  - '=='
```

---

## Operators Order

```yaml
type: BlanksChallenge
key: 8aa686fc32
```

`@context`


`@code1`
```{r}
 20 {{_fun1}} 2 {{_fun2}} 4 {{_fun3}} 8
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
  - 'a'
  - 'b'
  - 'c'
fun1:
  - '-'
fun2:
  - '**'
fun3:
  - '+'
```

`@distractors`
```yaml
fun1:
  - '+'
fun2:
  - '*'
fun3:
  - '/'
```

---

## Calculate Multiplier

```yaml
type: MultipleChoiceChallenge
key: add3f67f97
```

`@assignment1`
If you had a 10% interest rate starting with $100, how would you calculate the return after one month?

`@options1`
- 100 * 10%
- [100 * ( 1 + 10/100)]
- 100 * 10/100
- 100 * 1 + 10%/100

---

## One Month Mult

```yaml
type: BlanksChallenge
key: f2ab2fbbc7
```

`@context`
What would be the correct way to calculate the returns over one month with a fixed interest rate?

`@code1`
```{r}
{{var1}} <- {{var2}} {{_fun1}} {{_var3}}
{{var1}}
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
 - 'x'
 - 'y'
 - 'z'
var2:
 - '100'
 - '200'
 - '500'
fun1:
 - '*'
var3:
 - '1.10'
 - '1.05'
```

`@distractors`
```yaml
fun1:
 - '**'
 - '+'
var3:
 - '1.075'
 - '1.03'
 - '1.045'
```

---

## Multiple Months

```yaml
type: OutputChallenge
key: bef427dbcd
```

`@context`
Calculating stock returns over multiple months where the interest rate doesn't change can be done using the `**` operator.

`@code1`
```{r}
100 * {{var1}} ** {{var2}}

```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
 - '1.05'
 - '1.10'
 - '1.15'
var2:
 - '2'
```

---

## Variable Class

```yaml
type: OutputChallenge
key: 167oSz8A19yBt
```

`@context`


`@code1`
```{r}
class({{var1}})
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
  - '"FALSE"'
  - '"TRUE"'
  - 'TRUE'
  - 'FALSE'
  - '1'
  - '0'
  - '2 < 3'
  - '"2 > 3"'
```

---

## Numeric Type

```yaml
type: BlanksChallenge
key: 9f5268eb7c
```

`@context`


`@code1`
```{r}
x <- class({{_var1}})
x
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
  - '24'
```

`@distractors`
```yaml
var1:
  - '23 < 24'
  - '"23"'
  - '22L'
  - '"24"'
```

---

## Logical Type

```yaml
type: OutputChallenge
key: 48b1a6c822
```

`@context`


`@code1`
```{r}
answer <- {{var1}}
class(answer)
```

`@pre_challenge_code`
```{r}

```

`@variables`
```yaml
var1:
 - '"FALSE"'
 - 'FALSE'
 - '0'
 - '0L'
```
