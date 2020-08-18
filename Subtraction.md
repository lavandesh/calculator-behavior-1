# Subtraction 

## Scenario: Subtraction of two positive numbers

Given The calculator is ON

When I type in "positive number"
And I press "minus"
And I type in another "positive number"
And I press "equals"

Then I see the "subtracted number" as the result

## Scenario: Subtraction of two negative numbers

Given The calculator is ON

When I type in "negative number"
And I press "minus"
And I press "Open Bracket"
And I type in another "negative number"
And I press "Close Bracket"
And I press "equals"

Then I see the "subtracted number" as the result

## Scenario: Subtraction of fractions

Given The calculator is ON

When I press "open bracket"
And type in "Fractional number"
And press "close bracket"
And I press "minus"
And I press "open bracket"
And type in another "Fractional number"
And press "close bracket"
And I press "equals"

Then I see the "subtracted Fraction" as the result

## Scenario: Subtraction of positive and negative number

Given The calculator is ON

When I type in "Positive number"
And I press "minus"
And I press "Open Bracket"
And I type in another "negative number"
And I press "Close Bracket"
And I press "equals"

Then I see the "subtracted number" as the result

## Scenario: Subtraction of more than 2 numbers

Given The calculator is ON

When I type in "number"
And I press "minus"
And I type in another "positive number"
And I press "minus"
And I type in another "positive number"
And I press "equals"

Then I see the "subtracted number" as the result

## Scenario: Identity operation

Given The calculator is ON

When I type in "number"
And I press "minus"
And I type in Zero
And I press "equals"

Then I see the same "number" as the result

## Scenario: Converse operation

Given The calculator is ON

When I type in "positive number"
And I press "minus"
And I type in another "positive number"
And I press "equals"
And I press "clear"
And I type in "positive number"
And I press "minus"
And I type in another "positive number"
And I press "equals"

Then I see the different "subtracted number" as the result in both case
