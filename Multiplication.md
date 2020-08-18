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

## Scenario: Simple multiplication

## Scenario: Rational multiplication

## Scenario: Decimal & integer multiplication

## Scenario: More than two numbers multiplication

Given the calculator is ON

## Scenario: Range of operand exceeds allowed limit

Given the calculator is ON

## Scenario: Pressing "multiply button" more than once

Given the calculator is ON

## Scenario: Interleaving operators (Press *, then press /, then press +)

Given the calculator is ON

## Scenario: Decimal value capping

Given the calculator is ON
