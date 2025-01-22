# Expo AsyncStorage: Null Handling for Missing Keys

This repository demonstrates a common error when using AsyncStorage in Expo applications and provides a solution.  The problem arises when attempting to access a key that doesn't exist; AsyncStorage returns `null`, leading to potential crashes if not carefully addressed.  The solution showcases the correct method for handling the null case.

## Bug
Attempting to access a property of `null` when `AsyncStorage.getItem()` returns `null` leads to an application crash.

## Solution
Implement a check for null before using the retrieved value, ensuring the application handles missing keys gracefully.
