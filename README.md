# Image Recognition

![image](https://github.com/user-attachments/assets/dec48702-128e-43e6-a6ea-56cc38413b78)

![image](https://github.com/user-attachments/assets/99759e71-c9cf-445d-a35d-45f694ecabe3)

## Prompt

const get2dPrompt = () =>
    `Detect ${
      targetPrompt
    }, Output a json list where each entry contains the 2D bounding box in "box_2d" and ${
      labelPrompt || 'a text label'
    } in "label".`

### Prompt Example

Character Recognition and Spatial Analysis

Identify the Hanzi characters written by the user.
Analyze the shape, size, proportions, stroke order, stroke direction, and relative positions of strokes in the characters.
Validation of Writing

Compare the recognized characters with the standard Unicode for Hanzi, including reference stroke order and correct character structure.
Detect errors such as:
Incorrect stroke order.
Incorrect stroke shape or direction.
Imbalanced character proportions.
Incorrect placement of character elements.
Scoring and Feedback

Provide a score on a scale (e.g., 0–100) for each written character.
If there are errors, offer detailed descriptions of:
The type of error.
The specific part of the character with the mistake.
Provide an example of the correct character writing for reference, either as an image or a step-by-step description.
Summary Evaluation

Display an overall score based on the average performance of all written characters.
List characters with errors, including a breakdown of specific mistakes and corrections.
Offer tips for improving handwriting, such as focusing on specific stroke orders or character proportions.

