# CC103 Parking Fee System

A Java-based console application designed to manage parking transactions for the **BulSU CICT Parking Space**. This project was developed as a final requirement for **CC103 (Computer Programming 1)**.

## Project Overview
This program simulates a parking management system. It handles the entire flow of a parking transaction: from vehicle entry and validation to fee calculation, payment processing, and official receipt generation.

## Key Features

### Vehicle Management
* **Input Validation:** Validates plate numbers (Format: 3 letters + 4 numbers) and prevents duplicate entries of the same vehicle.
* **Vehicle Types:** Supports distinct billing rates for Cars, Motorcycles, and SUVs/Trucks.
* **Time Tracking:** Accepts 24-hour format input and calculates duration automatically.

### Fee Calculation Logic
* **Grace Period:** First 30 minutes are free.
* **Hourly Rates:** Calculates fees based on base rates + succeeding hourly rates.
* **Overnight Parking:** Detects and calculates fees for overnight stays.
* **Penalties:** Automatic P200.00 penalty for lost tickets.

### Admin & Security
* **Login System:** Secure entry with username/password (Default: `BSIS` / `123`).
* **Credential Management:** Allows the logged-in admin to change their username and password.
* **System-Wide Summary:** Generates a session report tracking:
    * Total vehicles processed (by type).
    * Total revenue and cash tendered.
    * Total discounts and penalties applied.
    * Average income per vehicle.

## Limitations/Recommendations
* **Re-login:** The user must re-login after changing login credentials.
* **Plate Number Duplication:** In a real-world scenario, a vehicle can park multiple times, thus making the duplicate checker pointless.
* **Contact Information:** Developer contact information is missing.

## Technologies Used
* **Language:** Java (JDK 8+)
* **Input/Output:** `java.util.Scanner` for input, `System.out.printf` for formatted output.

## How to Run

1.  **Download/Clone:** Download the `PFS.java` file or clone this repository.
   
2.  **Compile:** Open your terminal/command prompt and navigate to the folder containing the file.
    ```bash
    javac PFS.java
    ```
    
3.  **Run:**
    ```bash
    java PFS
    ```

## Usage Guide

1.  **Login:** Enter the default credentials to access the Main Menu.
2.  **New Parking Record:** Select `[1]` to process a vehicle. Enter the plate, type, time-in, and time-out.
3.  **Payment:** The system will display the amount due. Enter the cash tendered to generate the receipt.
4.  **View Summary:** Select `[2]` at any time to see the total statistics for the current session.
5.  **Member Info & About:** Select `[3]` to recognize the developers who made this project.
6.  **Change Username/Password:** Select `[4]` to change user login credentials.
7.  **Exit:** Select `[5]` to terminate the program.

## 👤 Authors

**BS Information Systems | CC103 - Computer Programming 1** **Bulacan State University (BulSU)**

* **[Christian Jabez J. San Andres](https://github.com/Occial)**
* **Dexter E. Payabyab**
* **Adrian R. Fabian**
* **John Ashley R. Dela Rosa**
* **Christian Michael T. Banzuela**

---
*This project is for educational purposes only.*
