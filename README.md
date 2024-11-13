# NLP_AssignmentOne
Assignment project of NLP course at University of Bologna.

# TODO
### Instructions
~1. **Download** the `A1/data` folder.~ 
~2. **Load** the three JSON files and encode them as pandas dataframes.~
~3. **Generate hard labels** for Task 1 using majority voting and store them in a new dataframe column called~ ~`hard_label_task1`. Items without a clear majority will be removed from the dataset.~
~4. **Filter the DataFrame** to keep only rows where the `lang` column is `'en'`.~
~5. **Remove unwanted columns**: Keep only `id_EXIST`, `lang`, `tweet`, and `hard_label_task1`.~
6. **Encode the `hard_label_task1` column**: Use 1 to represent "YES" and 0 to represent "NO".   -Jana


### Instructions
- **Remove emojis** from the tweets.
- **Remove hashtags** (e.g., `#example`).
- **Remove mentions** such as `@user`.
- **Remove URLs** from the tweets.
- **Remove special characters and symbols**.
- **Remove specific quote characters** (e.g., curly quotes).
- **Perform lemmatization** to reduce words to their base form.
