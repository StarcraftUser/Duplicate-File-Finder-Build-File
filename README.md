# Duplicate-File-Finder-Build-File

Duplicate File Finder Build File

---

## License

This project is licensed under the Apache License 2.0.

### Libraries Used

This project uses several external libraries, each with its own license.

The libraries included in this project are:

- **NPOI** (NPOI.Core.dll, NPOI.OpenXml4Net.dll, NPOI.OOXML.dll, NPOI.OpenXmlFormats.dll) - Apache License 2.0  
- **ICSharpCode.SharpZipLib** (ICSharpCode.SharpZipLib.dll) - MIT License  
- **System.* libraries** (System.Runtime.CompilerServices.Unsafe.dll, System.Numerics.Vectors.dll, System.Memory.dll, System.Buffers.dll) - MIT License  
- **ZString** (ZString.dll) - MIT License  
- **Microsoft.IO.RecyclableMemoryStream** (Microsoft.IO.RecyclableMemoryStream.dll) - MIT License  
- **Ude** (Ude.dll) - MPL License 1.1  
- **MultiMapWapperX64.dll** (Custom Library by [StarcraftUser]) - MIT License

For more information about these libraries, visit their respective repositories.

### Apache License 2.0

This project is licensed under the Apache License, Version 2.0 (the "License");  
you may not use this file except in compliance with the License.  
You may obtain a copy of the License at:

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
See the License for the specific language governing permissions and limitations under the License.

---

한국어 설명은 아래 블로그에서 확인하실 수 있습니다.

For detailed Korean instructions, please refer to the blog below.

https://intelhurricane.tistory.com/133

---


## Introduction to Duplicate File Finder

Recently, the prices of HDDs and SSDs have been soaring since the New Year, making storage increasingly burdensome.

With prices rising more than threefold, managing storage space has become more important than ever.

In order to ease the burden of storage space, even just a little, I decided to create my own duplicate file checker.

I had tried several duplicate file finders I found through Google, but they had some inconveniences:  
- The UI was too small, making it difficult to view large file lists at a glance.  
- The programs randomly designated one file as the “original” and deleted the rest, which made it hard to control the process as I wanted.  
- Even if search results were saved, they could only be opened within that specific program.  

To improve these shortcomings, I developed **Duplicate File Finder**.

---

## Key Features

- **Dark Mode Support**: Reduces eye strain, making long-term use more comfortable.
<img src="./images/1.png" width="600">
<img src="./images/2.png" width="600">

- **Single Hash Value Check**: Calculate the hash value of a file to use as a unique identifier.
<img src="./images/3.png" width="600">

- **Compare Two File Hashes**: Directly compare the hash values of two files to determine if they are identical.
<img src="./images/4.png" width="600">

- **Folder Comparison**: Specify two folders to find common files and delete them if necessary.
<img src="./images/5.png" width="600">

- **Duplicate File Search**: Scan multiple drives or designated folders to find and remove duplicate files.
<img src="./images/6.png" width="600">

---
## Deletion Options

After scanning for duplicates, pressing the delete button will display the following options.
<img src="./images/7.png">

When using the folder comparison feature, the following deletion options window will appear.
<img src="./images/8.png">

- Delete files from the left folder
- Delete files from the right folder
- Delete from both folders

Before deletion, a warning message will appear, requiring agreement that “responsibility for deletion lies with the user” before proceeding.

<img src="./images/9.png">

---
## Performance Control

<img src="./images/10.png" width="600">

You can set the number of simultaneous processes during duplicate file scanning.  
For example, if there are 3 paths and the concurrency is set to 20, a total of 60 files will be scanned simultaneously.  
However, setting the number too high may overload the HDD or CPU, so appropriate values are recommended.

---

## Result Saving

<img src="./images/11.png">
<img src="./images/12.png" width="800">
<img src="./images/13.png" width="800">

Search results can be saved as TXT or Excel files, which can then be viewed and edited.  

---

## Saving File Editing

<img src="./images/14.png" width="600">
<img src="./images/15.png" width="600">

A result editor allows you to extract or exclude extensions, change priorities, and designate the desired path as the original file.  
For example, if you switch the order of the Z and P drives, the P drive files can be designated as originals, while Z drive files are set for deletion.  
<img src="./images/16.png" width="800">

Using the deletion options in this state will neatly remove duplicate files from the Z drive.
<img src="./images/17.png">

---

## Drive Letter Modification

If drive letters change, they can be updated in the settings window.  
After modification, you must restart or reset the program and reload the list for changes to take effect.  
If you do not reset, the file list will not be refreshed.
<img src="./images/18.png" width="600">
<img src="./images/19.png" width="800">

---

## Load

After making changes, please restart the program or reload the list after initialization to apply the changes.  
Without initialization, the file list will not be updated.
<img src="./images/20.png" width="600">

---

## Additional Features

Duplicate File Finder goes beyond simply finding duplicate files by offering extra functionality: 

- **Empty Folder Deletion**  
<img src="./images/21.png" width="600">
 
- **Registry Difference Extractor**  
<img src="./images/22.png" width="600">

- **Limited Language Support**: Korean, English, Japanese, and Hebrew are experimentally included.  
&nbsp; (Since translations are AI-generated, they may sound slightly awkward.)  
<img src="./images/23.png" width="600">

- **Result Saving and Editing Tools**: Designed to let users manage files in their preferred way.  
<img src="./images/24.png" width="600">

---

## Conclusion

This tool runs on **Windows environments with .NET Framework 4.7.2 installed**.  
If you discover any **bugs in the program**, I would greatly appreciate it if you could report them.  
Please note that any issues **caused by program malfunctions are the responsibility of the user**.  
As **storage space becomes increasingly precious**, I hope this tool helps **slim down your storage and ease the burden**, even just a little.  

**That concludes the explanation. Thank you.**

**[Download Link](https://github.com/StarcraftUser/Duplicate-File-Finder-Build-File/releases)**

---
