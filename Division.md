# Division

## Scenario: Division by 0 when operand 1 is any number

Given the calculator is ON

When I enter any 'number'
and press 'divide'
and press 'zero'
and press equals

then display 'Invalid operation'

## Scenario: Divide 0 by any number

Given the calculator is ON

When I press 'zero'
and press 'divide'
and enter any 'number' except zero
and press equals

then display 'zero'

## Scenario: Sign rules for operands

Given the calculator is ON

When I press 'open bracket' and enter 'number with
sign'
And press 'close bracket' and press 'divide'
And again press 'open bracket' and enter another
'number along with sign'
And press 'close bracket' and press 'equals'

then display the result with sign

## Scenario: Division isn't symmetric

Given The calculator is ON

When I type in "positive number"
And I press "divide"
And I type in another "positive number"
And I press "equals"
And I press "clear"
And I type in "positive number"
And I press "divide"
And I type in another "positive number"
And I press "equals"

Then I see the different "number" as the result in
both case

## Scenario: Division when both operands are 0

Given the calculator is ON

When I press 'zero'
and press 'divide'
and press 'zero'
and press equals

then display 'Not Defined'

## Scenario: Recurring decimal case

Given the calculator is ON

When I divide two numbers to give recurring decimal
and press equals

then display result with decimal points
rounded up to 8 digits

## Scenario: Multiple times "/" is pressed

Given the calculator is ON

When I enter a 'number'
and I press 'divide' more than once
and I enter another 'number'
and press equals

Then display 'divided number' as a result

## Scenario: Interleaving of multiple operators

Given the calculator is ON

When I enter a 'number'
and press 'divide'
and press 'subtract'
and press 'add'
and enter 'another number'
and press equals

Then display 'added number' as a result

## Scenario: When operand 2 is not present

Given the calculator is ON

When I enter a 'number'
and I press 'divide'
and press equals

Then display 'same number' as a result

## Scenario: Division by any/all operands being fractions

Given the calculator is ON

When I press 'open bracket' and enter 'fractional
number'
And press 'close bracket' and press 'divide'
And again press 'open bracket' and enter another
'fractional number'
And press 'close bracket' and press 'equals'

then display the result in decimals up to 8 places

## Scenario: Division of multiple numbers (eg: 4/5/6/7)

Given the calculator is ON

When I type in "positive number"
And I press "divide"
And I type in another "positive number"
And I press "divide"
And I type in another "positive number"
And I press "equals"

Then I get "number got by moving left to right
one by one division" as a result
