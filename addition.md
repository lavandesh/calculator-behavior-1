# Addition

## Scenario: Addition of two positive numbers

Given The calculator is ON

When I type in "positive number"
And I press "plus"
And I type in another "positive number"
And I press "equals"

Then I see the "added number" as the result

## Scenario: Addition of two negative numbers

Given The calculator is ON

When I type in "negative number"
And I press "plus"
And I press "Open Bracket"
And I type in another "negative number"
And I press "Close Bracket"
And I press "equals"

Then I see the "added number" as the result

## Scenario: Addition of fractions

Given The calculator is ON

When I press "open bracket"
And type in "Fractional number"
And press "close bracket"
And I press "plus"
And I press "open bracket"
And type in another "Fractional number"
And press "close bracket"
And I press "equals"

Then I see the "added Fractional" as the result

## Scenario: Addition of positive and negative number

Given The calculator is ON

When I type in "Positive number"
And I press "plus"
And I press "Open Bracket"
And I type in another "negative number"
And I press "Close Bracket"
And I press "equals"

Then I see the "added number" as the result

## Scenario: Addition of decimals

Given The calculator is ON

When I type in "Decimal number"
And I press "plus"
And I type in another "Decimal number"
And I press "equals"

Then I see the "Added Decimal number" as the result

## Scenario: Typing operator more than once

Given The calculator is ON

When I type in "positive number"
And I press "plus" and again press "plus"
And I type in another "positive number"
And I press "equals"

Then I see the "added number" as the result

## Scenario: Addition of more than 2 numbers

Given The calculator is ON

When I type in "number"
And I press "plus"
And I type in another "positive number"
And I press "plus"
And I type in another "positive number"
And I press "equals"

Then I see the "added number" as the result

## Scenario: Adding numbers where the result goes out of range

Given The calculator is ON

When I type in "largest positive number"
And I press "plus"
And I type in another "largest positive number"
And I press "equals"

Then I see the "Out Of Range" as the result

## Scenario: 6+* as input

Given The calculator is ON

When I type in "positive number"
And I press "plus"
And I press "Multiply"
And I press "equals"

Then I see the same "positive number" as the result

## Scenario: Identity operation

Given The calculator is ON

When I type in "number"
And I press "plus"
And I type in Zero
And I press "equals"

Then I see the same "number" as the result

## Scenario: Converse operation

Given The calculator is ON

When I type in "positive number"
And I press "plus"
And I type in another "positive number"
And I press "equals"
And I press "clear"
And I type in "positive number"
And I press "plus"
And I type in another "positive number"
And I press "equals"

Then I see the same "added number" as the result in both case