# Time Adder

This project is a Python function to add time to a given starting time, considering AM/PM format and optional day of the week. It handles arithmetic operations on time values and determines the resulting time after adding a specified duration.

## How to Use

### Prerequisites

- Python 3.x installed on your system.
- No additional libraries are required.

### Running the Function

1. **Save the function** as `time_adder.py` or any name you prefer.
2. **Open a terminal or command prompt**.
3. **Navigate to the directory** where the function is saved.
4. **Run the function** by executing the following command:

    ```bash
    python time_adder.py
    ```

### Function Details

The function `add_time` performs the following tasks:

- **Time Addition**:
  - Takes a starting time (`start`) and a duration (`duration`) to add.
  - Computes the resulting time after adding the duration to the starting time.

- **AM/PM Handling**:
  - Adjusts AM/PM as necessary when the calculated time exceeds 12 hours.

- **Day Calculation**:
  - Optionally accepts a day of the week (`d_day`) to compute the day after adding the duration.

### Example

Here are some examples demonstrating how to use the `add_time` function:

```python
print(add_time('3:30 PM', '2:12'))
print(add_time('11:55 AM', '3:12'))
print(add_time('2:59 AM', '24:00'))  # (next day)
print(add_time('11:59 PM', '24:05'))
print(add_time('8:16 PM', '466:02'))
print(add_time('3:30 PM', '2:12', 'Monday'))  # Monday
print(add_time('2:59 AM', '24:00', 'saturDay'))  # Sunday (next day)
print(add_time('11:59 PM', '24:05', 'Wednesday'))
print(add_time('8:16 PM', '466:02', 'tuesday'))  # 102s
