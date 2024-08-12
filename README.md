

---

# Python Automated Email Birthday Wisher

## Overview

The Python Automated Email Birthday Wisher is a script designed to automatically send personalized birthday wishes to your contacts via email. This program reads contact details from a CSV or Excel file, checks for upcoming birthdays, and sends out customized email greetings using an SMTP server. It's an ideal tool for automating birthday reminders, ensuring that your loved ones or clients receive timely and thoughtful wishes.

## Features

- **Automated Email Sending:** Automatically sends personalized birthday wishes via email.
- **CSV/Excel Data Handling:** Reads contact information, including names, email addresses, and birthdates, from a CSV or Excel file.
- **Customizable Templates:** Allows customization of the email message template for a more personalized touch.
- **SMTP Configuration:** Easily configurable SMTP settings for secure email sending.
- **Daily Execution:** Can be scheduled to run daily, ensuring no birthday is missed.

## Requirements

- Python 3.x
- `pandas` for data handling
- `smtplib` for sending emails
- `email.mime` for constructing the email content

You can install the necessary packages using pip:

```bash
pip install pandas
```

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/automated-email-birthday-wisher.git
   cd automated-email-birthday-wisher
   ```

2. **Prepare the Contacts File:**

   - Create a `contacts.csv` or `contacts.xlsx` file with the following columns:
     - `Name`
     - `Email`
     - `Birthday` (in `YYYY-MM-DD` format)

3. **Configure SMTP Settings:**

   - Open the `config.py` file (or wherever you've placed your SMTP settings) and update it with your email provider's SMTP settings, such as:
     ```python
     SMTP_SERVER = 'smtp.gmail.com'
     SMTP_PORT = 587
     EMAIL_ADDRESS = 'your-email@example.com'
     EMAIL_PASSWORD = 'your-email-password'
     ```

4. **Customize the Email Template:**

   - Modify the `birthday_message.txt` file or the in-script template to personalize your birthday wishes.

5. **Run the Script:**

   - You can run the script manually:
     ```bash
     python birthday_wisher.py
     ```

   - Or set it up as a scheduled task to run daily using cron (Linux/Mac) or Task Scheduler (Windows).

## Usage

- Ensure your contacts file is up to date.
- Customize the email template to fit your style.
- Run the script daily to check for birthdays and send emails automatically.

## Contributing

Contributions are welcome! If you have any ideas for improvements or want to fix bugs, feel free to fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or suggestions, feel free to contact me at princetrojan@proton.me

---
