# ChatApp-ReactNative-
A simple chatting app built with React Native. It allows users to send and receive messages in real-time.

## What it does
This app provides a basic chat interface where users can create accounts, add friends, and engage in private conversations. It's a great starting point for anyone looking to build a messaging app with React Native.

## Installation
To get started, clone this repository and install the required dependencies:
```bash
npm install
```
Then, link the necessary packages:
```bash
npx react-native link
```
## Running the app
To run the app on an emulator or physical device, use the following command:
```bash
npx react-native run-android
```
or
```bash
npx react-native run-ios
```
## Example usage
Here's a quick example of how to send a message:
```javascript
import React, { useState } from 'react';
import { View, Text, TextInput, Button } from 'react-native';

const ChatScreen = () => {
  const [message, setMessage] = useState('');

  const handleSendMessage = () => {
    // Send message logic here
    console.log(`Sending message: ${message}`);
  };

  return (
    <View>
      <TextInput
        placeholder="Type a message"
        value={message}
        onChangeText={setMessage}
      />
      <Button title="Send" onPress={handleSendMessage} />
    </View>
  );
};
```
Note: This is just a basic example and you'll need to implement the actual messaging logic.