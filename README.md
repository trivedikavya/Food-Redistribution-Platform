# Food Redistribution Platform

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

## Overview
The Food Redistribution Platform is an innovative **console-based application** designed to address food waste and hunger issues. It connects donors, NGOs, and volunteers in a streamlined process to facilitate the efficient redistribution of surplus food to those in need. The platform incorporates blockchain technology for data integrity and AI-powered matching to optimize food distribution.

## Features

### Basic Features

1. User Management
   - Multi-role user system (Donor, NGO, Volunteer, Admin)
   - Secure registration with input validation
   - Login system with hashed password storage

2. Donation Management
   - Add and track food donations
   - View available donations
   - Claim donations (for NGOs)

3. Task Management
   - Create delivery tasks for claimed donations
   - View and accept tasks (for Volunteers)
   - Track task completion

4. Reward System
   - Point-based system for user actions
   - Leaderboard to display user rankings

5. Notifications
   - Crisis mode alerts
   - Admin-sent notifications

### Advanced Features

1. Blockchain Integration
   - Basic blockchain implementation for donation tracking
   - Ensures data integrity and transparency

2. AI-powered Food Matching
   - Uses TF-IDF and cosine similarity algorithms
   - Matches donations with NGO needs for optimal distribution

3. Crisis Mode
   - Toggleable mode for prioritizing urgent donations
   - Affects notification system and task prioritization

## Technologies Used

1. Python 3.7+
2. JSON (for data storage)
3. hashlib (for password hashing)
4. scikit-learn (for TF-IDF vectorization and cosine similarity)
5. numpy (for numerical operations)
6. re (for input validation using regular expressions)


## File Structure
```
│-- main.py                         # Main entry point  (Just run this all things will work easy [Use replit])
│-- food_redistribution_data.json    # Stores application data (will create Automatically)
│-- README.md                        # Project documentation

```
-- Replit is a online compiler which is next level for python 

## Outputs

## 1 Chat-Bot 

```python
Bot: Hello!
You: what is your name
Bot: I'm ChatBot K-1.1.
:You your owner is
Bot: My owner is KAVYA TRIVEDI.
You: what time it is
Bot: Your system has watch plz check there .
You: your age
Bot: I'm just a bot, so I don't have an age, but if you're asking for my version, it's 2.
You: how's the weather today
Bot: The weather is currently good if
you want to know more just open the window of your room.
You: how are you
Bot: I'm just a bot, I don't have feelings, but thanks for asking!
You: your owner contact information
Bot: My owner is KAVYA TRIVEDI.
You: yeah but its contact information
Bot: You can contact Kavya Trivedi on Instagram: @kavyatrivedi.og or on GitHub: trivedikavya
You: How many girls are there in your staff
Bot: All are married brother
You: How to start investing
Bot: For that you need money 
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
- Through that rewards you can get benefits in Tax(if Gov collab) or can buy something through that rewards.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any queries, reach out to `kavyatrivedi931@gmail.com`. 🚀
