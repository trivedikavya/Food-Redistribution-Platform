# Food Redistribution Platform

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

## Overview
The **Food Redistribution Platform** is a blockchain-backed system designed to efficiently manage food donations, distribution, and volunteer coordination. It ensures security, transparency, and incentivizes participation through a reward system.

## Features
### General Features
- User roles: **Donor, NGO, Volunteer, Admin**
- Blockchain-based **donation storage** for security
- **Crisis Mode** for emergency prioritization
- **Leaderboard & Reward System** to encourage participation

### Donor Features
- Add food donations
- View available donations
- Earn reward points for contributions

### NGO Features
- View and claim donations
- Assign tasks for volunteers
- Receive notifications

### Volunteer Features
- View available delivery tasks
- Accept and complete tasks
- Earn points for completing tasks

### Admin Features
- Manage users and donations
- Activate/Deactivate Crisis Mode
- Send notifications to users
- View Leaderboard

## Technologies Used
- **Python** (Core programming language)
- **Blockchain** (For secure donation storage)
- **JSON** (For data storage)
- **hashlib**, **json**, **os**, and **sys** (built-in Python libraries) 
-  the only external dependency is **tabulate**

## Installation
### Prerequisites
Ensure you have Python 3.7 installed.

### Steps
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/food-redistribution.git
   cd food-redistribution
   ```
2. Install required dependencies:
   ```sh
   pip install tabulate
   ```
3. Run the application:
   ```sh
   python food_redistribution.py
   ```

## File Structure
```
│-- main.py                         # Main entry point of the application
│-- food_redistribution_data.json    # Stores application data (created automatically)
│-- README.md                        # Project documentation

```


## Contributing

We welcome contributions to improve the Food Redistribution Platform! Here are some ways you can contribute:

1. Report bugs and suggest features by opening issues
2. Submit pull requests with bug fixes or new features
3. Improve documentation
4. Share ideas for enhancing the platform

Please read our [Contributing Guidelines](CONTRIBUTING.md) for more details.

## Future Enhancements

- Web or mobile app interface
- Real-time notifications
- Integration with mapping services for efficient routing
- Partnerships with local businesses and organizations

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any queries, reach out to `kavyatrivedi931@gmail.com`. 🚀
