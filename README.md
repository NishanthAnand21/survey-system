# PHP Simple Survey

This survey system is developed in PHP. It is lightweight yet highly capable of handling extensive survey data.

## Screenshots

### Interface

The user interface is designed to be clean and modern, minimizing distractions to help users focus on providing better responses.

![Survey interface](image.png "Survey interface")

### Administration Panel

The backend panel provides an overall view of survey results. Each survey submission triggers an email notification, and the results page offers a comprehensive view of the collected responses.

![Results](image-1.png "Results")

The administration panel also allows for the addition and editing of survey questions. Currently, there are six different question types available:
- Yes or No
- Text Box
- Paragraph
- Multiple Choice
- Expanded Multiple Choice
- Checkboxes
- Number Slider

![Add a question](image-2.png "Add a question")

### User Support

While multi-user support is not yet available, it is planned for future updates. Currently, one administrator account is created during installation. The goal is to support three types of accounts: admin (created at install), full access, and read-only.

![User support](image-3.png "User support")

## Installation

1. Modify the `connect()` function inside `class/Connection.php` to include your database credentials. For example:
	```php
	function connect(){
		return mysqli_connect(
			'localhost', // Database server
			'db_user',   // Database user
			'db_pass',   // Database password
			'db_name'    // Database name
		);
	}
	```
2. Run `install.php` to complete the setup.
