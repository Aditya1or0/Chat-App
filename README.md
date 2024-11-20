# Chat-App

A real-time chat application built with React.js and Firebase. This app allows users to securely log in, chat, send images, change profile pictures, set a bio, and search for friends, enhancing communication and user interaction.

## Features

- **Real-Time Messaging**: Users can send and receive messages in real-time.
- **Secure Authentication**: Implemented login and signup functionality with Firebase Authentication.
- **Profile Customization**: Users can update their profile pictures and bio.
- **Image Sharing**: Send images during conversations.
- **Friend Search**: Search and connect with other users.
  
## Tech Stack

- **Frontend**: React.js, Firebase (Authentication, Firestore, Storage)
- **Backend**: Firebase (Firestore for data storage)
- **Deployment**: Vercel

## Demo

You can try out the live application here: [Chat-App Demo](https://chat-app-nine-ruby.vercel.app/)

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Aditya1or0/Chat-App.git
cd Chat-App
```

### 2. Install dependencies

Run the following command to install the required dependencies:

```bash
npm install
```

### 3. Set up Firebase

- Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
- Set up Firebase Authentication, Firestore, and Firebase Storage.
- Add the Firebase configuration to your app:
  
In the `src/firebase.js` file, add your Firebase configuration object:

```js
import firebase from 'firebase/app';
import 'firebase/auth';
import 'firebase/firestore';
import 'firebase/storage';

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const firebaseApp = firebase.initializeApp(firebaseConfig);
const db = firebaseApp.firestore();
const auth = firebaseApp.auth();
const storage = firebaseApp.storage();

export { db, auth, storage };
```

Make sure to replace the placeholders with your actual Firebase project details.

### 4. Run the app

Once the setup is complete, you can start the application by running:

```bash
npm start
```


## Contributing

If you'd like to contribute to this project, please fork the repository, create a new branch, and submit a pull request.

## License

This project is open-source and available under the MIT License.

## Acknowledgements

- **React.js**: For building the user interface.
- **Firebase**: For providing real-time database, storage, and authentication services.
- **Vercel**: For deployment.

---
