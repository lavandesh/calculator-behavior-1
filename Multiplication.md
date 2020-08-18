# Multiplication

## Scenario: Result overflow

Given the calculator is ON

When I multiply two sufficiently large numbers
to give a 11 digit or longer number
but not beyond the largest integer possible

Then display the number with scroll feature

## Scenario: Multiplication of Numbers with Signs

Given the calculator is ON

When I press 'open bracket' and enter 'negative number'
And press 'close bracket' and press 'multiply'
And again press 'open bracket' and enter another 'negative number'
And press 'close bracket' and press 'equals'

Then I see multiplication result with positive sign

## Scenario: Multiplication by Zero

## Scenario: Multiplication by 1

## Scenario: Multiplication of Decimals

## Scenario: Multiplication of Irrationals

Given the calculator is ON

When I enter an 'irrational number'
and press multiply
and enter another 'irrational number'
and press equals

then display the result in decimals upto 8 places

## Scenario: Simple multiplication

## Scenario: Rational multiplication

Given the calculator is ON

When I press 'open bracket' and enter 'rational number'
And press 'close bracket' and press 'multiply'
And again press 'open bracket' and enter another 'rational number'
And press 'close bracket' and press 'equals'

then display the result in decimals upto 8 places

## Scenario: Decimal & integer multiplication

## Scenario: More than two numbers multiplication

Given the calculator is ON

When I type in "positive number"
And I press "multiply"
And I type in another "positive number"
And I press "multiply"
And I type in another "positive number"
And I press "equals"

Then I get "multiplied number" as a result

## Scenario: Range of operand exceeds allowed limit

Given the calculator is ON

When I enter a 'number' larger than the biggest integer

Then display 'too large to handle' as a result

## Scenario: Pressing "multiply button" more than once

Given the calculator is ON

When I enter a 'number'
and I press 'multiply' three time consecutively
and I enter another 'number'
and press equals

Then display 'multiplied number' as a result

## Scenario: Interleaving operators (Press *, then press /, then press +)

Given the calculator is ON

When I enter a 'number'
and press 'multiply'
and press 'divide'
and press 'add'
and enter 'another number'
and press equals

Then 'added number' is displayed as a result

## Scenario: Decimal value capping

Given the calculator is ON

When I multiply two numbers
whose multiplication has more than 9 digits
after decimal point

Then display multiplied number rounded upto 8 digits
