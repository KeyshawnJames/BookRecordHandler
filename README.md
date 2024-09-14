# BookStoreHandler

The project is designed to build a program that processes and validates book records from CSV files. It performs three main tasks:

1. Syntax Validation: The program reads book records from input CSV files and checks for syntax errors such as missing fields or unknown genres. Valid records are then organized by genre and saved into separate CSV files.

2. Semantic Validation: It then examines the valid records for data accuracy, such as checking for valid ISBNs, correct prices, and appropriate publication years. Errors are logged in a separate file.

3. Serialization: Finally, the program converts the valid book records into Java objects and saves them into binary files for efficient storage and future access.

The purpose is to ensure the data is correctly formatted, accurately recorded, and efficiently stored.

This project is split into three parts: 

Part 1: Syntax Validation and File Partitioning
In this part, you developed a method that reads book records from several CSV-formatted files, validating the syntax of each record. The program checks for common syntax errors such as missing fields, too many or too few fields, and unknown genres. If a syntax error is found, the error details are recorded in a syntax_error_file.txt. Valid book records are categorized based on their genre and stored into separate CSV files, corresponding to eight predefined genres.

Part 2: Semantic Validation and Serialization
In Part 2, you extended the program to handle semantic validation of the book records. After reading the genre-specific CSV files created in Part 1, the program checks each record for errors such as invalid ISBN numbers, incorrect prices, or invalid years. Records that fail these checks are recorded in a semantic_error_file.txt, while semantically valid records are converted into Book objects. These objects are then serialized and stored as binary files for future use.
