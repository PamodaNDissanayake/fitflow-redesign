# FitFlow AI Service

## Purpose

Generate personalized workout suggestions and support
consented cloud inference when required.

## Proposed Technologies

- Python
- FastAPI
- Suitable machine learning models

Mobile on-device inference uses LiteRT or ML Kit through
frontend platform adapters.

## Workout Inputs

- Fitness goals
- Experience level
- Available time
- Available equipment
- Relevant user-provided limitations
- Permitted workout history and feedback

## Expected Outputs

- Suggested exercises
- Estimated workout duration
- Plain-language recommendation reasons
- Alternative exercises
- Model version

## Nutrition Support

A suitable food recognition model may suggest food labels
and confidence values.

Users must confirm the food and portion before saving.
Nutrient estimates require a separate nutrient data source.
Image recognition alone does not provide reliable calories
or portion sizes.

## Privacy and Reliability

- Accept requests only from authorized backend services.
- Process only the information needed for the request.
- Keep meal images on the device by default.
- Require explicit consent for cloud image processing.
- Provide manual logging when recognition is unavailable.
- Return a curated workout fallback when inference fails.
- Validate model outputs before presenting recommendations.

## Status

Planning stage. No trained model or running AI service
is included in this repository.