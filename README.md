# Optimization-Based-Automation-Scheduling-via-Mathematical-Modeling
--------------------------
Problem Statement:

There are 45 employees working as production operators to produce lamp. Each day, the company has a production target that is divided between weekdays and weekends with the following details:
  - The target on weekday is to complete 6000 units.
  - The target on weekend is to complete 5000 units.

Based on this information, each operator has the same individual daily target which is to complete 200 units per day, in accordance with the company’s established standards. This target is essential to ensure the achievement of the overall daily production output.

However, the process of creating work schedules is still done manually by the HR team and production supervisors using spreadsheets and conventional records. Since the scheduling is done manually and without a supporting system, the process becomes highly complex and prone to errors.

Therefore, the HR and production supervision teams require assistance in generating schedules automatically based on several constraints as follows:

- There are 3 shifts where each shift consists of 8 working hours.
  - Shift 1 = 07:00 - 15:00
  - Shift 2 = 12:00 - 20:00
  - Shift 3 = 16:00 - 24:00
- Each employee should work at least one shift per day.
- Each employee should work only for 5 days each week and should have 2 days week off.
- No employees should work more than 5 consecutive days during any period.
- No employees should work with pattern "Day Off, Working, Day Off" consecutive days.
- Each employee only work with 1 shift type every week.
- If employees get night shift (shift 3), employees do not work in morning shift in the next day or in next shift.
- If employees request leave in the specific day, the total working day per week will reduce with total days requested for leave.

!Notes: The following cases were created based on assumed scenarios for the purpose of model development.
  ----------------------
Methodology:
- Install pulp library in your jupyter notebook
  !pip install pulp
- Convert the problem statement into mathematical equation
- The program is success if the status = "Optimal"

Result:
- A dataframe that contains information abut employees including shift type they work, days off, etc.
  ----------------------------
Tech:
- Jupyter Notebook / Google Colab
- Python
- pulp, pandas, and numpy library
