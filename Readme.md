# Voting Application

## Project Overview
The **Voting Application** is a socket programming project implemented in Python. This system allows authenticated users to cast their votes securely. The server manages multiple client connections using concurrent threads, ensuring that each client can vote once and only once. 

## Table of Contents
1. Project Analysis
2. Requirements
3. Tools Used
4. How to Run
5. How to Login
6. Workflow Description
7. Test Cases
8. Conclusion

## Project Analysis
This project is based on TCP socket programming, where a server handles multiple clients through concurrent threads. The key features include:
- Authentication of clients (voters).
- Ability for voters to cast a vote only once.
- Multithreading to handle multiple client connections simultaneously.
- Storage of registered voter information and vote counts.

## Requirements
**Python Libraries**:
- `pandas`
- `tkinter`
- `socket`
- `subprocess`

## Tools Used
- **Programming Language**: Python
- **Connection**: Socket Programming
- **Protocol**: TCP
- **User Interface**: python-tkinter
- **Data Storage**: CSV files
- **Data Updates**: python-pandas
- **OS Calls**: python-subprocess

## How to Run
1. Open the terminal/command prompt.
2. Navigate to the `Voting` folder.
3. Run the following command:
4. A new home page window should open.
5. Login as Admin and run the server.
6. Register voters and proceed with casting votes.

## How to Login
- **Admin Login**:
- Admin ID: `Admin`
- Password: `admin`

- **Voter Login**:
- Use voter IDs: `10001` to `10005`
- Password: `abcd`
- Otherwise Remove the voter IDs from admin portal and remove the before IDs and create the new one's.

Ensure that the server is running before voters attempt to log in.

## Workflow Description
1. Open the terminal and run `python homePage.py`.
2. Login as Admin and press `Run Server` to start the server.
3. Register voters, note the Voter ID, and use it for logging in as a voter.
4. Voters can log in and cast votes.
5. Admin can check the votes using the `Show Votes` button.

## Test Cases
- **Test Case 1**: Successful login and vote casting.
- **Test Case 2**: Error handling for multiple votes by the same client.
- **Test Case 3**: Handling concurrent voting by multiple clients (up to 6 at the same time).

## Conclusion
This project demonstrates the implementation of socket programming with Python, multithreading to handle multiple client connections, and the synchronization of threads to ensure secure and reliable voting.

## Database
- **Voter Info**: CSV file storing registered voter details.
- **Candidate Info**: CSV file storing candidate details.

