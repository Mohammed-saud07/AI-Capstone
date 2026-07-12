# AI Workflow Comparison

## Overview

For this exercise, I implemented the same settings form feature using two different prompting approaches. The goal was to compare the quality of AI-generated code when using a vague prompt versus a detailed, structured prompt.

### Round One – Vague Prompt

I asked the AI to "Create a React settings form with validation." The generated code produced a working form with basic input fields and simple validation. However, it lacked detailed error handling, accessibility improvements, and comprehensive validation. The component worked, but it required significant manual review to identify missing edge cases and improve the user experience.

### Round Two – Precise Prompt

For the second implementation, I provided detailed requirements including file locations, validation rules, accessibility requirements, controlled React components, expected behavior, and a verification step requesting tests. The resulting code was much more structured. Form fields included appropriate labels, validation messages were clearer, the submit button was disabled until the form became valid, and the overall component organization was easier to understand and maintain.

## Differences Observed

The second implementation included stronger validation logic, cleaner component structure, improved accessibility, and more consistent coding style. It also followed the requested constraints more closely, reducing the amount of manual editing required. The generated code was easier to review because the AI had explicit expectations to follow.

## AI Mistake I Caught

In the first implementation, the AI accepted an invalid email format and did not properly disable the submit button when required fields were empty. I corrected the validation logic before considering the feature complete. This demonstrated that AI-generated code should always be reviewed and verified rather than accepted without inspection.

## Lessons Learned

This exercise showed that prompt quality has a direct impact on code quality. A detailed specification leads to more reliable output, fewer review cycles, and better maintainability. Going forward, I will provide clear constraints, expected behavior, verification steps, and project-specific rules whenever using AI to generate code.
