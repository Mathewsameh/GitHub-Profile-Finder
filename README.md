# 🐙 GitHub User Profile Finder

A simple Python project that uses the **GitHub REST API** to retrieve and display public information about any GitHub user by entering their username.

## 📌 Project Overview

This project allows users to quickly view essential information about a GitHub profile without manually visiting the GitHub website.

It uses Python's `requests` library to send an HTTP GET request to the GitHub API, process the JSON response, and display the user's profile details in the terminal.

## ✨ Features

- 🔍 Search for GitHub users by username.
- 👤 Display the GitHub username and full name.
- 👥 Show the number of followers.
- 📦 Display the number of public repositories.
- 📝 Show the number of public gists.
- 🔗 Provide a direct link to the user's GitHub profile.
- ⚠️ Handle invalid usernames and connection errors.
- ⏱️ Use a request timeout to prevent waiting indefinitely for a response.
- 📊 Display the HTTP status code for debugging and response checking.

## 🛠️ Technologies Used

- **Python 3**
- **Requests Library**
- **GitHub REST API**
- **JSON**
- **Exception Handling**

## 📋 Requirements

- Python 3.x installed on your computer.
- An active internet connection.
- The `requests` library.

## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/github-user-profile-finder.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Navigate to the Project Folder

```bash
cd github-user-profile-finder
```

### 3. Install Dependencies

```bash
pip install requests
```

### 4. Run the Program

```bash
python main.py
```

If your Python file has a different name, replace `main.py` with your actual filename.

## 💻 Example Usage

Enter a GitHub username when prompted:

```text
Enter GitHub username: torvalds

Status Code: 200
Username: torvalds
Name: Linus Torvalds
Followers: [current follower count]
Public Repositories: [current repository count]
Public Gists: [current gist count]
Profile URL: https://github.com/torvalds
```

*Note: Follower and repository counts change over time. The actual output depends on the data returned by GitHub's API.*

## 🔄 How It Works

1. The program asks the user to enter a GitHub username.
2. It removes unnecessary whitespace from the input.
3. It constructs the GitHub API endpoint using the username.
4. It sends a GET request with a 10-second timeout.
5. It checks the HTTP status code:
   - `200 OK`: Retrieves and displays the user's profile information.
   - `404 Not Found`: Displays an error message if the user does not exist.
   - Other status codes: Displays a general error message.
6. It handles request-related exceptions if the connection fails or the request encounters an error.

## 📚 What I Learned

Through this project, I practiced:

- Making HTTP requests using Python.
- Working with REST APIs.
- Processing JSON data.
- Handling HTTP status codes.
- Using `try` and `except` for error handling.
- Accessing dictionary values returned by an API.
- Building interactive command-line applications.

## 🔮 Future Improvements

- Display the user's bio, location, and account creation date.
- Show the user's most popular repositories.
- Add input validation for empty usernames.
- Improve error handling for API rate limits.
- Save profile information to a JSON file.
- Build a graphical user interface.

## 📖 Useful Resources

- [GitHub REST API Documentation](https://docs.github.com/en/rest)
- [GitHub Users API](https://docs.github.com/en/rest/users/users#get-a-user)
- [Python Requests Documentation](https://requests.readthedocs.io/en/latest/)

## 👨‍💻 Author

**YOUR NAME**

- GitHub: [@YOUR-USERNAME](https://github.com/YOUR-USERNAME)

---

⭐ If you find this project useful, consider giving the repository a star!
