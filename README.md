# codepath_homework_week7-8

# Project 7 - WordPress Pentesting

Time spent: 20 hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. XSS Vulnerability 1
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: 
    -  <img src="Comment Vulnerability.gif" alt="Comment Vulnerability">
  - [ ] Steps to recreate: 
    - Go to a post to leave a comment
    - Post the infected code into the comment
    - Click on the Submit button
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 2. XSS Vulnerability 2
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough:
    -  <img src="Vulnerability 2.gif" alt="Image Vulnerability">
  - [ ] Steps to recreate: 
    -  Add new post 
    -  Click add media
    -  Insert your image that has the infected code as the name
    -  Select Attachment Page under Link To (in the bottom right hand corner)
    -  Insert it into the post
    -  Publish and view the post
    -  When you click on the image, the exploit is revealed
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 3. Title Widget Vulnerability
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.4
  - [ ] GIF Walkthrough: 
    -  <img src="Vulnerability 3.gif" alt="Title Vulnerability"> 
  - [ ] Steps to recreate: 
    -  As an admin, go to the Appearances tab and select Widgets
    -  Click Text Widget
    -  Add infected code into the Title Box under Meta 
    -  Refresh to the main page and the alert will pop up
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with ScreenToGIF

## Notes

- I had issues with the Kali linux screen freezing
- I also had an issue with Vagrant where 'vagrant up' would not work but that was resolved by uninstalling and reinstalling vagrant 

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
