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

## Outputs & Working

### Application Startup 

```python
Welcome to the Food Redistribution Platform
1. Login
2. Create Account
3. Exit
Enter your choice: 
```
### User Registration & Login 
```python
Enter your name: leo
Enter your email: leooo@example.com
Set your password (min 8 characters, include numbers or symbols): Pass@123
Select Your Role:
1. Donor
2. NGO
3. Volunteer
4. Admin
Enter your choice: 1
Account created successfully!

FOR Login 

Enter your email: leooo@example.com
Enter your password: Pass@123
Welcome back, leo !
```
### Donor Role: Sample Console Output

```python
Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 2

Enter your name: John Doe
Enter your email: john@example.com
Set your password: *****

Select Your Role:

Donor
NGO
Volunteer
Admin
Enter your choice: 1

Account created successfully!

Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 1

Enter your email: john@example.com
Enter your password: *****

Welcome back, John Doe!

Dashboard

Add Donation
View Donations
View Notifications
View Rewards
View Leaderboard
Logout
Enter your choice: 1

Add Donation
Enter the food item: Bread
Enter the quantity: 10 loaves
Enter the expiry date (YYYY-MM-DD): 2025-01-15

Donation added successfully!

Dashboard

Add Donation
View Donations
View Notifications
View Rewards
View Leaderboard
Logout
Enter your choice: 2

Current Donations

Bread - 10 loaves (Expires: 2025-01-15)

Dashboard

Add Donation
View Donations
View Notifications
View Rewards
View Leaderboard
Logout
Enter your choice: 4

Your current reward points: 25

Dashboard

Add Donation
View Donations
View Notifications
View Rewards
View Leaderboard
Logout
Enter your choice: 5

Leaderboard

John Doe - 25 points

Dashboard

Add Donation
View Donations
View Notifications
View Rewards
View Leaderboard
Logout
Enter your choice: 0

Logging out...
```

### Admin Role: Sample Console Output

```python
Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 2

Enter your name: AdminUser
Enter your email: admin@example.com
Set your password: *****

Select Your Role:

Donor
NGO
Volunteer
Admin
Enter your choice: 4

Account created successfully!

Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 1

Enter your email: admin@example.com
Enter your password: *****

Welcome back, AdminUser!

Admin Dashboard

View All Users
View All Donations
Activate/Deactivate Crisis Mode
View Leaderboard
Manage Notifications
Logout
Enter your choice: 1

All Registered Users:

John Doe (Donor)
Helping Hands NGO (NGO)
Alex Smith (Volunteer)

Admin Dashboard

View All Users
View All Donations
Activate/Deactivate Crisis Mode
View Leaderboard
Manage Notifications
Logout
Enter your choice: 2

All Donations:

Bread - 10 loaves (Donor: John Doe | Claimed by: Helping Hands NGO)
Rice - 25 kg (Donor: Jane Donor | Pending)

Admin Dashboard

View All Users
View All Donations
Activate/Deactivate Crisis Mode
View Leaderboard
Manage Notifications
Logout
Enter your choice: 3

Crisis Mode Status: OFF

Do you want to activate Crisis Mode? (yes/no): yes

Crisis Mode Activated! Notifications sent to all users.

Admin Dashboard

View All Users
View All Donations
Activate/Deactivate Crisis Mode
View Leaderboard
Manage Notifications
Logout
Enter your choice: 5

Send Notification to All Users:
Enter your message: Urgent! Volunteers are needed for emergency food distribution.

Notification sent successfully!

Admin Dashboard

View All Users
View All Donations
Activate/Deactivate Crisis Mode
View Leaderboard
Manage Notifications
Logout
Enter your choice: 0

Logging out... 
```
###  NGO Role: Sample Console Output

```python
Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 2

Enter your name: Helping Hands NGO
Enter your email: ngo@example.com
Set your password: *****

Select Your Role:

Donor
NGO
Volunteer
Admin
Enter your choice: 2

Account created successfully!

Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 1

Enter your email: ngo@example.com
Enter your password: *****

Welcome back, Helping Hands NGO!

Dashboard

View Donations
Claim Donation
View Notifications
View Leaderboard
Logout
Enter your choice: 1

Current Donations

Bread - 10 loaves (Expires: 2025-01-15)
Rice - 25 kg (Expires: 2025-01-20)

Dashboard

View Donations
Claim Donation
View Notifications
View Leaderboard
Logout
Enter your choice: 2

Claim Donation
Enter the donation number you want to claim: 1

Donation claimed successfully! Thank you for making a difference.

Dashboard

View Donations
Claim Donation
View Notifications
View Leaderboard
Logout
Enter your choice: 3

Your Notifications

Crisis Mode is now active! Prioritize urgent donations.
Donor John Doe added 10 loaves of Bread available for pickup.

Dashboard

View Donations
Claim Donation
View Notifications
View Leaderboard
Logout
Enter your choice: 4

Leaderboard

Helping Hands NGO - 50 points
John Doe - 25 points

Dashboard

View Donations
Claim Donation
View Notifications
View Leaderboard
Logout
Enter your choice: 0

Logging out...
```
###  Volunteer Role: Sample Console Output 

```python
Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 2

Enter your name: Alex Smith
Enter your email: alex.volunteer@example.com
Set your password: *****

Select Your Role:

Donor
NGO
Volunteer
Admin
Enter your choice: 3

Account created successfully!

Welcome to the Food Redistribution Platform

Login
Create Account
Exit
Enter your choice: 1

Enter your email: alex.volunteer@example.com
Enter your password: *****

Welcome back, Alex Smith!

Dashboard

View Available Tasks
Accept Delivery Task
View Notifications
View Leaderboard
Logout
Enter your choice: 1

Available Tasks

Pick up 10 loaves of Bread from John Doe and deliver to Helping Hands NGO.
Pick up 25 kg of Rice from Jane Donor and deliver to Hope Foundation.

Dashboard

View Available Tasks
Accept Delivery Task
View Notifications
View Leaderboard
Logout
Enter your choice: 2

Enter the task number to accept: 1

Task accepted successfully! Please complete the delivery.

Dashboard

View Available Tasks
Accept Delivery Task
View Notifications
View Leaderboard
Logout
Enter your choice: 3

Your Notifications

Crisis Mode Activated! Volunteers are needed urgently.
Task #1 assigned. Please deliver Bread to Helping Hands NGO.

Dashboard

View Available Tasks
Accept Delivery Task
View Notifications
View Leaderboard
Logout
Enter your choice: 4

Leaderboard

Alex Smith - 30 points
Helping Hands NGO - 50 points

Dashboard

View Available Tasks
Accept Delivery Task
View Notifications
View Leaderboard
Logout
Enter your choice: 0

Logging out...
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
