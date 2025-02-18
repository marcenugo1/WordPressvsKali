# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. XSS Posts Cross Site scripting 
  - [ ] Summary: The add new Posts section is vulnerable to XSS scripting 
  - Vulnerability types: xss
  - [ ] Steps to recreate: 
  1. Create a new post 
  2. add some xss scripting on the post 
  3. click on preview 
  4. xss scripting is executed. 
  - [ ] GIF Walkthrough: 
  ![1](https://user-images.githubusercontent.com/9220950/160225133-998444fa-8594-46fe-8599-25d94aabfb00.gif)
  
  ### 2. XSS Pages Titles Cross Site scripting 
  - [ ] Summary: The pages title section is vulnerable to XSS scripting 
  - Vulnerability types: xss
  - [ ] Steps to recreate: 
  1. Go to any of the pages in the pages section. 
  2. Edit the title of the page selected and add a xss scripting attack
  3. click on preview 
  4. xss scripting is executed. 
  - [ ] GIF Walkthrough: 
  ![2](https://user-images.githubusercontent.com/9220950/160225533-d8370469-01d9-44bf-bd94-4483828faeb1.gif)
  
    ### 3. XSS attachment name images CVE-2016-5834
  - [ ] Summary: This vulnerability enables an attacker to add in the name of an attached image xss scripting
  - Vulnerability types: xss
  - Tested in version: 4.2
  - Fixed in version: 4.5.2
  - [ ] Steps to recreate: 
  1. Go to any of the pages in the pages section. 
  2. Click on add media
  3. Upload an image that has a name with xss scripting. example: <img src=xss onerror=alert(document.cookie)>.jpg
  4. change attachment display settings as attachment page. 
  - [ ] GIF Walkthrough: 
  ![3](https://user-images.githubusercontent.com/9220950/160227337-c120ba5b-851a-433a-a4f5-7e0e05d80c6e.gif)


  

Describe any challenges encountered while doing the work

It was very challenging to setup everything on a mac book with m1. Virtualbox is still not able to create VMs with the m1 processor. 

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
