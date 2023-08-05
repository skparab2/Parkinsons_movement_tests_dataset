# Parkinsons_movement_tests_dataset

Results from 31 participants (13 Parkinson's, 18 Non-Parkinson's) from a movement test at https://skparab1.github.io/pd


## Data arrangement
- Rows (except for header): represents a participant
- Columns: represent features
  - Status: Parkinson's status (PD or non-PD)
  - Feature 1. Mean deviation from centerline when tracing straight line (fraction of screen height)
  - Feature 2. Amount of time taken to trace straight line (miliseconds)
  - Feature 3. Amount of time taken to trace straight line with respect to window width (miliseconds)
  - Feature 4. Percentage of points traced inside straight line
  - Feature 5. Number of points traced inside straight line with no regard to time taken
  - Feature 6. Amount of time taken to trace sine wave (miliseconds)
  - Feature 7. Amount of time taken to trace sine wave with respect to window width (miliseconds)
  - Feature 8. Percentage of points traced inside sine wave
  - Feature 9. Number of points traced inside sine wave with no regard to time taken
  - Feature 10. Amount of time taken to trace spiral (miliseconds)
  - Feature 11. Amount of time taken to trace spiral with respect to window width (miliseconds)
  - Feature 12. Percentage of points traced inside spiral
  - Feature 13. Percentage of points traced inside spiral with no regard to time taken
  - Feature 14. False presses when prompted with a constant key
  - Feature 15. False presses when prompted with a semi-random(random between 2 letters) key
  - Feature 16. False presses when prompted with a random key
  - Feature 17. Total false presses from all tests
  - Feature 18. Average false presses from all tests
  - Feature 19. Average response time when prompted with a constant key (miliseconds)
  - Feature 20. Sum of response times when prompted with a constant key (miliseconds)
  - Feature 21. Average response time when prompted with a semi-random(random between 2 letters) key (miliseconds)
  - Feature 22. Sum of response times when prompted with a semi-random(random between 2 letters) key (miliseconds)
  - Feature 23. Average response time when prompted with a random key (miliseconds)
  - Feature 24. Sum of response times when prompted with a random key (miliseconds)
  - Feature 25. Number of correctly pressed keys when prompted with a constant key
  - Feature 26. Number of correctly pressed keys when prompted with a semi-random(random between 2 letters) key
  - Feature 27. Number of correctly pressed keys when prompted with a random key
  - Feature 28. Number of correctly pressed keys when prompted with a random key with respect to average response time
  - Feature 29. Maximum deviation from centerline when tracing straight line (percentage of screen height)
  - Feature 30. Maximum deviation from centerline when tracing straight line without regard to window height (pixels)
  - Feature 31. Net accumulated deviation from centerline when tracing straight line (percentage of screen height)
  - Feature 32. Total accumulated deviation from centerline when tracing straight line (percentage of screen height)
  - Feature 33. Avg of absolute values of deviation from centerline when tracing straight line (percentage of screen height)
- An optimized model based on this data was a RandomForestClassifier trained on features 1, 7, 10, 18, 20, 28. These features were deemed as important using an ExtraTreeClassifier importance predictor.
