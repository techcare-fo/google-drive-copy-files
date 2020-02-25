# google-drive-copy-files

Script to copy large amounts of files in google drive, can be used to backup/copy from one account to another

## Script properties

| Name              | Description                                                                                                                       | Default |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------- |
| maxFilesSoft      | Number of files to copy in one go, soft limit will finish a folder even if limit is reached                                       | 100     |
| rescheduleSeconds | Number of seconds to wait until script is rescheduled after maxFilesSoft limit is reached                                         | 10      |
| rescheduleTimeout | Number of seconds to wait until script is restarted if it fails or times out (This is cancelled if the script itself reschedules) | 2400    |
| sourceFolderId    | Id of source folder [How to find](https://ploi.io/documentation/mysql/where-do-i-get-google-drive-folder-id)                      |         |
| targetFolderId    | Id of target folder                                                                                                               |         |

## How to use

Copy the script to [Google Apps Script](https://script.google.com/home/start). Set the script properties and then run start function.

