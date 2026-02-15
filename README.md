# Crop Management System

A simple Crop Management System built using Python and Tkinter. This application allows users to manage crop records, including inserting manual records, bulk inserting random records, updating records, and displaying the last 20 records from a MySQL database.Here we can manage crops on the basis of inserting and adding bulk amount of crop

## Features

- Insert manual crop records
- Bulk insert 100,000 random crop records
- Update existing crop records
- Display the last 20 crop records

## Requirements

- Python 3.x
- MySQL server
- Tkinter (usually included with Python)
- Faker library

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/crop-management-system.git
    ```

2. Navigate to the project directory:
    ```sh
    cd crop-management-system
    ```

3. Install the required Python packages:
    ```sh
    pip install mysql-connector-python faker
    ```

4. Set up the MySQL database:
    - Create a database named `crop_management`.
    - Create a table named `crops` with the following structure:
      ```sql
      CREATE TABLE crops (
          id INT AUTO_INCREMENT PRIMARY KEY,
          crop_name VARCHAR(255) NOT NULL,
          planting_date DATE,
          harvest_date DATE,
          growth_stage VARCHAR(255),
          pest_control_measures TEXT,
          yield_prediction INT
      );
      ```

## Usage

1. Run the application:
    ```sh
    python cropgui.py
    ```

2. Use the GUI to manage crop records:
    - Insert manual records by filling in the input fields and clicking "Insert Record".
    - Bulk insert 100,000 random records by clicking "Insert 100,000 Random Records".
    - Update existing records by selecting a record from the table, modifying the input fields, and clicking "Update Record".
    - View the last 20 records in the table.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
