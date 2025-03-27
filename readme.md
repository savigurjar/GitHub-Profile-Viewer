# GitHub Profile Finder

A React application that allows users to search for GitHub profiles by username and generate a list of random GitHub profiles.

## Features
- Search for a specific GitHub user by entering a username.
- Generate a specified number of random GitHub profiles.
- Fetches data from the GitHub API.
- Displays profile pictures and usernames with links to their GitHub profiles.
- Optimized with `useCallback` to prevent unnecessary function re-creation.
- Handles errors and invalid inputs gracefully.

## Installation

### Prerequisites
- Node.js and npm installed
- A React project set up

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/github-profile-finder.git
   cd github-profile-finder
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the development server:
   ```sh
   npm start
   ```

## Usage
1. **Generate Random Profiles:**
   - Enter a number (e.g., 10) in the input field.
   - Click the "Display Profiles" button to fetch that number of random GitHub profiles.
   - The profiles will be displayed with usernames, avatars, and links to their GitHub pages.

2. **Search for a Specific Profile:**
   - Enter a GitHub username in the search bar.
   - Click the "Search Profile" button to fetch the user's details.
   - If the profile exists, it will be displayed.
   - If the user is not found, an error message will appear.

## Code Explanation
### **Main Components**
- **useState:** Manages state for profiles, search queries, and loading status.
- **useCallback:** Prevents unnecessary re-creation of API-fetching functions.
- **useEffect:** Calls the `generateProfile()` function on initial render.

### **Functionality**
- `generateProfile(count)`: Fetches a list of random GitHub profiles based on the specified count.
- `provideProfile(name)`: Fetches and displays a single GitHub profile based on the entered username.
- `useEffect()`: Ensures that random profiles are loaded when the component mounts.

## Technologies Used
- React.js
- JavaScript (ES6+)
- GitHub API
- HTML
- CSS (for basic styling)

##API
 "https://api.github.com/users?per_page=10"
  https://api.github.com/users/taylorotwell
 `https://api.github.com/users?since=6000&per_page=20`

