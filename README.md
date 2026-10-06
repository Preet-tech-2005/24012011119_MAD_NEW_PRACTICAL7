# Practical 7

**Enrollment Number:** 24012011119

## Aim

To develop an Android application that fetches person information in JSON format from an online API and saves the received data into an SQLite database.

## Description

This practical demonstrates how an Android application can retrieve JSON data from a remote API using the internet. The application uses `HttpURLConnection` to send an HTTP request and Kotlin's `CoroutineScope` to perform the network operation in the background.

After receiving the JSON response, the data is parsed and converted into `Person` objects. The retrieved persons are displayed in the application using a `RecyclerView` with a custom adapter. The application also uses SQLite through `SQLiteOpenHelper` to store the fetched information locally, allowing the data to remain available even when the device is offline.

The `Person` class implements `Serializable`, which allows person information to be passed between different activities using `Intent` extras, such as sending location details to a Map activity.

## Key Concepts and Technologies

* **JSON Parsing:** Converting JSON response data into usable person objects.
* **Networking:** Using `HttpURLConnection` to send HTTP GET requests and retrieve data from an online API.
* **Coroutines:** Running network-related tasks in the background using `CoroutineScope(Dispatchers.IO)` so the main UI thread remains responsive.
* **RecyclerView:** Showing the list of retrieved persons efficiently using a custom `PersonAdapter`.
* **SQLite Database:** Storing person information locally using `SQLiteOpenHelper`, including operations such as inserting, retrieving, and updating records.
* **Serialization:** Passing custom `Person` objects between activities using `Intent` and `Serializable`.
* **Permissions:** Adding internet permission in the Android manifest to allow the application to access the remote API.

## Screenshots

<div align="center">
  <!-- Replace 'screenshot1.png' and 'screenshot2.png' with your actual screenshot file names and place them in the root directory alongside this README or update the path to the images -->
  <img src="Screenshots/Layout 1.png" alt="App Screenshot - Light Mode" width="300" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="Screenshots/Layout 2.png" alt="App Screenshot - Dark Mode" width="300" />
</div>
