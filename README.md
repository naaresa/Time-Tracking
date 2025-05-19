# Time Tracking Program
A Time Tracking Program in Python

## Business Problem
Nana recently started a consulting business where he is paid based on the number of hours and minutes he works on client projects. He needs a time tracking program to enter the date and time he starts and finishes a task, calculate the hours spent, and determine the amount earned at $5 per hour. For example, if Nana works from 11:00 AM to 1:30 PM on Monday, 27th July, he earns 2.5 × $5 = $12.50. The program should store task details in a CSV file for future reference.

## Task
Write a program to help Nana track his earnings. The program should:
- Calculate the hours spent on a task.
- Compute the amount earned based on the hours.
- Store task details (task type, start/end times, hours, and amount) in a CSV file.
- Display a summary of the task and payment.

## Approach
1. Created a `getDatetime()` function to collect start and end datetimes from the user in the format `dd/mm/yyyy HH:MM`, with validation for correct input.
2. Developed a main `timeTracker()` function that calls `getDatetime()` to assign start and end dates.
3. Computed hours spent using the `total_seconds()` method from the `datetime` module to find the duration and convert it to hours.
4. Calculated earnings by calling `pay_per_hour()`, which multiplies hours by $5 and rounds to two decimal places.
5. Stored task details (task type, start date, end date, hours, amount) in a list and wrote it to `timetracking.csv`.
6. Printed a summary string with the task duration and payment.

## Installation
The program requires Python 3.x and uses standard libraries (`datetime` and `csv`), so no additional installations are needed. To run the script, ensure you have Python installed:
```bash
python --version
```

## Usage
1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-username/Time-tracking.git
   ```
2. **Navigate to the Directory**  
   ```bash
   cd Time-Tracking
   ```
3. **Run the Script**  
   ```bash
   Hourly_payment_tracker.py
   ```
4. **Follow Prompts**  
   - Enter the task type (e.g., "Consulting").
   - Enter start and end datetimes in `dd/mm/yyyy HH:MM` format (e.g., `27/07/2023 11:00`).
   - The program will output a summary (e.g., "Nana worked for 2.5 hours, between 2023-07-27 11:00:00 and 2023-07-27 13:30:00. He should be paid $12.5.") and save details to `timetracking.csv`.

## Output
The program generates:
- A console output summarizing the task, duration, and payment.
- A `timetracking.csv` file with columns: Task, Start Date, End Date, Hours, Amount.

## Contributing
Contributions are welcome! To contribute:
- Fork the repository.
- Create a new branch for your changes.
- Submit a pull request with a clear description.

Please open issues for bugs or suggestions.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author
- Theresa Gyamfi Allotey
