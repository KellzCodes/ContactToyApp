# ContactToyApp
Android App that displays Implicit Intents for Contact List

This app will demonstrate how to retrieve a list of contacts whose data matches all or part of a search string, using the following techniques:

## Match contact names
Retrieve a list of contacts by matching the search string to all or part of the contact name data. The Contacts Provider allows multiple instances of the same name, so this technique can return a list of matches.

## Match a specific type of data, such as a phone number
Retrieve a list of contacts by matching the search string to a particular type of detail data such as an email address. For example, this technique allows you to list all of the contacts whose email address matches the search string.

## Match any type of data
Retrieve a list of contacts by matching the search string to any type of detail data, including name, phone number, street address, email address, and so forth. For example, this technique allows you to accept any type of data for a search string and then list the contacts for which the data matches the string.

#### This app uses a [Cursor Loader](https://developer.android.com/reference/android/support/v4/content/CursorLoader.html) to retrieve data from the Contacts Provider. A CursorLoader runs its on a thread that's separate from the UI thread. This ensures that the query doesn't slow down UI response times and cause a poor user experience. For more information, see the Android training class [Loading Data in the Background](https://developer.android.com/training/load-data-background/index.html).
