---
description: Changelogs of the AMU project
---

# Changelog

## [12/05/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.45)

#### Improvements

* If title set to "Skipping Title" it will no longer try to search for it
* Added more logic to improve title matching
* Added around 80 more default alternative titles
* Added error handling for possible no internet connection

## [11/29/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.43)

#### New Features

* Added more default Alternative Titles
* Added time remaining for getting Manga ID's

#### Improvements

* Added additional logic for better search results
* Added some logic specific for Linux

#### Bug Fixes

* Fixed issue with values not getting reset when running the program more than once in a single session.

## [11/28/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.43)

#### New Features

* Added a alternative names feature. (You can now add a different title for the program to search for rather than the one from Kenmei)

## [11/24/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.35)

#### New Features

* Added a progress bar to show how far the program is currently into the program\
  Added a Time taken label that updates every second and keeps track of how long the program runs.

#### Improvements

* Changed how results of a manga search are printed. (Should not print duplicate results for each id)
* Changed how things printed in terminal to make it easy to read and understand. (Hopefully)
* Added a last chapter read and search link on Anilist for every Manga not found in the text file.
  * Also added the last chapter read for manga with multiple IDs

#### Bug Fixes

* Fixed issue where manga with some different punctuation was not getting recognized. Program now ignores any punctuation in titles.
* Fixed issue if no search result was given by pymoe it did not add it to Not Found Manga list.

## [11/23/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.35)

#### Improvements

* Sets gui theme to dark on default for linux. Tkinter is not able to properly get systems default color on linux platforms.
* Program now saves 5 text files of the Not found Manga and Multiple ID Manga in a seperate directory.

#### Bug Fixes

* Fixed problem in linux where the the "terminal" would go blank when it is getting updated.
* Fixed issue with program incorrectly getting csv file differences. Only now checks the (Title, Status, Last Chapter Read, Last Read At) columns.

## [11/21/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.1)

#### Improvements

* Changed print statements in terminal window (Should not look as cluttered as before, hopefully)

#### Bug Fixes

* Fixed issue program not getting correct type of status from api for manga. (Was getting the release status rather than the reading status on a users list)

## [11/19/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.0)

#### New Features

* Added fully functional GUI.
  * Program will no longer open up in a console. All print statements are run through the GUI.

## [11/18/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v2.0)

#### New Features

* Program now checks if the status between Kenmei and Anilist is different regardless of chapters read. And updated accordingly

## [11/15/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v1.5)

#### New Features

* Added check for if the manga was set to plan\_to\_read
* Added a way for user to have manga which has not been read for a certain time and set it to PAUSED

#### Bug Fixes

* Properly sets manga to PLANNING and PAUSED

## [11/14/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v1.4)

#### New Features

* Added universal api\_request function for Anilist API
* Program waits according to Anilist rate limit
* Added timing to keep track how long parts of the program takes to run

#### Improvements

* Increased max retries for getting manga id from pymoe

#### Bug Fixes

* Program properly writes out manga's with multiple id's
* Manga's are now updated to what the status was on Kenmei

## [11/13/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v1.3)

#### New Features

* Added a check to see if user wants entries to be private on Anilist.
* Added a sub directory in the directory of the program for keeping track of when and how many chapters were updated.

## [11/12/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/releases/tag/v1.2)

#### Improvements

* Added 1/3 of a second delay when updating manga in case so not too many requests might get sent to the api.

## [11/11/2023](https://github.com/RLAlpha49/Anilist-Manga-Updater/commit/3f618019b134a1aa86f052a2336bad91a5e22db3)

[Initial Program Release](https://github.com/RLAlpha49/Anilist-Manga-Updater/commit/34e6bd3018d55891789daa66162f4735d9f07791)
