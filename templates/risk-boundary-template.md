# Risk Boundary Template

Use this before implementation when a task touches an existing project with stable flows, unclear risks, or a strong temptation to "fix a little more while we are here".

The goal is not to describe every possible risk.

The goal is to make one thing explicit before coding starts:

what this round is allowed to change, and what this round must not touch.

## 1. Current Task

- What is the current request or delivery task:
- What is the single most important result of this round:
- If only one thing gets delivered this round, what should it be:

## 2. Stable Flow Baseline

- What existing flow is already working and should be treated as stable:
- Why is that flow not a good target for larger change right now:
- Does this round need to touch that flow directly:

## 3. High-Risk Zones

- Which modules, layers, or flows are high-risk in this round:
- Why are they high-risk:
- What is most likely to break if they are changed directly:

## 4. Lower-Risk Zones

- Which layers are safer to iterate on in this round:
- Why are they a better landing point:
- What is the smallest useful delivery that can be achieved only from these zones:

## 5. What This Round May Change

- Which pages, files, or layers are allowed to change:
- Which new components or wrappers are acceptable:
- Which low-risk cleanup is acceptable in this round:

## 6. What This Round Must Not Change

- Which pages, files, or layers are explicitly out of scope:
- Which structural cleanup is not part of this round:
- Which core flow, state machine, or data path must stay untouched:

## 7. Why Those Areas Stay Untouched

- What is the main reason not to touch them now:
- In which later round would they be more appropriate:
- What extra validation or rollback cost would be created if they were changed now:

## 8. Recommended Order

- What should be done first:
- What should be done next:
- At which point should implementation pause for validation:

## 9. Validation Focus

- Which user-visible path matters most in this round:
- Which edge cases should be checked carefully:
- Which signals would show that the change radius is getting too large:

## 10. Notes

- Explicitly excluded directions:
- Confirmed but postponed issues:
- Other notes:

## How To Use It

- Write the main delivery goal before writing the allowed change list.
- If the "must not change" section stays vague, the round boundary is still unclear.
- The most valuable part is usually not the risk list itself. It is the part that prevents unnecessary expansion.
