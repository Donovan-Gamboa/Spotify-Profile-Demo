# Spotify Profile Viewer

A simple web app to display Spotify profile data by connecting to the Spotify Web API. This app retrieves and showcases user profile details such as display name, profile picture, and playlists.

## Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

- A Spotify account (free or premium)
- [Spotify Developer Account](https://developer.spotify.com/) with an app registered to obtain the **Client ID** and **Client Secret**

### Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/spotify-profile-viewer.git
   cd spotify-profile-viewer
   ```

2. **Create a Spotify App**
   - Go to the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications) and create a new app.
   - Note down the **Client ID** and **Client Secret**.
   - Add a redirect URI in the app settings (e.g., `http://localhost:3000/callback`).

3. **Configure Environment Variables**
   Create a `.env` file in the root directory and add your Spotify credentials:
   ```env
   CLIENT_ID=your-client-id
   CLIENT_SECRET=your-client-secret
   REDIRECT_URI=http://localhost:3000/callback
   ```

4. **Install Dependencies**
   ```bash
   npm install
   ```

5. **Run the Application**
   ```bash
   npm start
   ```

6. **Login and Grant Permissions**
   - Navigate to `http://localhost:3000` in your browser.
   - Click "Connect with Spotify" to log in and grant permissions.
   - Your Spotify profile data, including your display name, profile image, and playlists, will be displayed.

## API Usage

This app uses the following Spotify Web API endpoints:
- `/me` – to fetch user profile data.
- `/me/playlists` – to retrieve user playlists.

## Built With

- [Express](https://expressjs.com/) – Web framework for Node.js
- [Spotify Web API](https://developer.spotify.com/documentation/web-api/) – To access user profile and playlist data

## License

This project is licensed under the MIT License.
