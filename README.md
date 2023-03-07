# expert-system-recommendr

In this project, I will provide a system that offers food suggestions to heart patients to help them follow a healthy diet.

This will be done by conducting a diagnosis of their health condition through a blood pressure measurement.

## First

the system will ask the patient to measure their blood pressure three times at different intervals and take the average of the results and store it in the result.

## Second

the diagnosis will be based on the result.

## Third

based on the previous table, if the result is Elevated or HBP1 or HBP2, then this person is a heart patient and the system will suggest meals according to the result.

If the result is Normal, then the person is healthy and can eat whatever they want.

We have set a certain limit for each of the nutritional values (calories, carbohydrates, sodium, etc.) allowed in one meal for the patient and reduce it by a certain percentage as the blood pressure increases, so the same meals are not suggested for patients with two different levels of elevated blood pressure.

## Fourth

after confirming that the person is ill and knowing the blood pressure level, the system will ask if they suffer from diabetes, then the carbohydrates will be reduced. The system will then ask if they have kidney diseases, then Cholesterol, Fats, and saturated Fats will be reduced.

## Fifth

for the meals, we have a dataset of 10,000 meals. We have identified these meals as facts and stored these facts in an array.

After diagnosing the disease and knowing the maximum allowed nutritional value in the meal, we will search the meal array for meals whose nutritional value equals or is less than the previous limits.

This produces several suitable meals for the patient, which are stored in an array and sorted according to their nutritional value from lowest to highest, with the priority of sorting for sodium, then saturated Fats, then Fats, then Cholesterol, then carbohydrates, then calories. Finally, ten suitable meals are randomly suggested.
