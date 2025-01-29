# Silent Image Insertion Failure in HTML

This repository demonstrates an uncommon bug in HTML where dynamically inserting an image with an invalid source path into the DOM results in a silent failure.  The image won't render, and no JavaScript errors are thrown in the console.  The solution involves robust error handling to detect and manage invalid image sources.

## Bug Description

The `bug.html` file contains a script that attempts to add an image element to the page with a non-existent source. This results in no visible error, but the image is not displayed. This type of silent failure can be difficult to debug.

## Solution

The `solution.html` file demonstrates how to mitigate this issue. It incorporates error handling to check the image's loading status and provides alternative behaviors (like displaying a placeholder image) if the source is invalid.