# Aaron Ciuffo - Resume

Featured Git Repositories

## Work Related Projects

### [PowerSchool PowerQuery](https://github.com/txoof/PowerQuery)

PowerSchool Student Information System (SIS) PowerQuery PL/SQL plugins for integrating course, teacher, student and parent data into D2L/Brightspace Learning Management System (LMS). There is no off-the-shelf integration between these products. A customized solution is required to maintain accurate synchronization of these two systems. This synchronization occurs regularly and ensures that staff, parents and students are connected to the appropriate classes and any changes to student schedules such as a schedule or class change are managed.

The queries are written in a combination of Oracle SQL and managed through XML documents. Once packaged and installed on the SIS server, the plugin can be accessed through automation processes and set to synchronize comma separated value (CSV) data to the D2l/Brightspace instance in the cloud. 

### [gdrive_audit](https://github.com/txoof/gdrive_audit)

Audit ownership of all files in a Google Drive folder.

GDrive Audit produces a google sheet that shows all the files within a folder and their owners. This tool can aid google super admins migrating folders into a Google Shared Drive. Run the audit tool to verify that all items contained within the shared folder are owned by the team and are suitable for migrating into a Google Shared Drive.

Remember: When super-admins migrate a folder into a Shared Drive all ownership of the files is transferred to the organization. This is strictly a ONE WAY process and cannot be undone. If items that are meant for organization-wide consumption are migrated, the rest of the organization will lose access. Each item must be individually restored to the original owner. There is no undo.

### [insertFiles](https://github.com/txoof/insertFiles)

Quikcly insert files iles by grade-level into Student Cumulative Folders on Google Drive. This can assist in adding standardized test scores, report cards or similar documents into Student Cumulative Folders.

### [PortfolioCreator](https://github.com/txoof/portfolioCreator)

Create student cumulative folders on Google Drive using Google FileStream and student information exports from PowerSchool.

### [codesign](https://github.com/txoof/codesign)

Python3 script for signing, packaging, notarizing and stapling Apple command line binaries using altool. This script only requires Python3 and uses only standard libraries.

This script is specifically targeted at codesigning, notarizing, creating .pkg files and stapling the notarization onto commandline tools written and compiled outside of Apple Xcode. This was created specifically for notarizing and signing python tools created with PyInstaller.

As of MacOS Catalina, all distributed binaries must be signed and notarized using an apple developer account. This account costs $99 per year. .

Apple's documentation for this process is ABSOLUTELY terrible. For a guide to doing this manually see [Signing_and_Notarizing_HOWTO](https://github.com/txoof/codesign/blob/main/Signing_and_Notarizing_HOWTO.md)

### [IMSCC_scripts](https://github.com/txoof/IMSCC_scripts)

Extract all regular files from Learning Management Platform Common Cartridge files (IMSCC). This can help you locate individual files that are contained within an IMSCC archive downloaded from platforms such as Canvas, Brightspace, Moodle or PowerSchool Learning.

### [pdfEdit](https://github.com/txoof/pdfEdit)

Edits individual PDF reports into a single file ready for Alert Solutions in PowerSchool.

Alert Solutions can read a large PDF file containing information on multiple students and parse that file into individual emails. To distinguish one record from the next Alert Solutions looks for the following text (exactly and with absolutely no flexibility) where XXXXXX is the student number: StudentID:XXXXXX

This script searches individual MAP test results in PDF Format or the line "Student ID: XXXXXX" and replaces it with the Alert Solutions expectation and then combines the edited PDFs into a single large PDF file that Alert Solutions can use.

### [pyPDF_split](https://github.com/txoof/pyPDF_split)

Split PDFs with multiple student records into individual PDFs. This can aide in preparing PDF files for mail merges or sharing in Google Drive.

pyPDF_split searches a PDF for the string StudentID:NNNNNNN and splits the PDF into individual PDFs in a sub-folder with the StudentID embedded in the new file name.

pyPDF_split can handle student IDs in the following formats:

StudentID:123456; StudentId:123456; STUDENTID:123456; studentid:123456
upper/lower case is ignored in all cases
Student ID:123456; Student ID: 123456
pyPDF_split pairs nicely with the insertFiles and create_folders scripts.



## Hobby Projects

 ### [PaperPi](https://github.com/txoof/PaperPi#paperpi-v3-)

PaperPi is a lovely, quiet, *slow internet* e-Paper radio. There are no loud colors, no busy animations, just a lovely selection of the information you want without buzz and distraction. PaperPi rotates through your choice of plugin screens at the pace you choose.

![PaperPi Video](https://github.com/txoof/PaperPi/blob/main/documentation/images/paperpiV3.gif)

### [ItsyBitsy Useless Machine](https://github.com/txoof/Useless_Machine)

***Absolutely Useless, Completely Necessary**

It's pretty useless. It defies logic and your will. It's a machine that has exactly one purpose, to turn its self off. For something so useful, why is it so entertaining?

![Usless Machine Animation](https://github.com/txoof/Useless_Machine/blob/main/Useless_Machine.gif)

 ### [Audio Sensor irBlaster](https://github.com/txoof/audioSensor)

 Let's face it: nobody knows how to operate your stereo receiver. Your kids, husband, sister-in-law all just want to start music playing and have sound come out of the speakers. It should just work*, not be an exercise in frustrated button mashing.

![irBlaster Image](https://github.com/txoof/audioSensor/blob/master/irBlaster.jpg)

It's a mystery which remote turns on the stereo. It's an even bigger mystery which button switches it so Spotify or the CD player plays. The irBlaster helps solve this problem by listening to two channels such as a CD Player and Media PC with Spotify, Movies, etc.

The irBlaster listens to the line-level audio over RCA cables. When it detects audio traffic on one of the channels, it sends a POWER ON Infrared (IR) code to the receiver, waits a few seconds for it to power up and then sends the IR code for the matching input. When there's no more audio traffic, it sends the POWER OFF IR code to the receiver.

### [epdlib](https://github.com/txoof/epdlib)

EpdLib is a library for creating dynamically scaled screen layouts for frame-buffered devices such as e-paper/e-ink displays. Complex layouts are defined as image, drawing or text blocks. Using epdlib blocks makes it trivial to develop for different disiplay resolutions as layouts are aware of thier resolution and scale the blocks dynamically to match the available area.

| | |
|-|-|
|![500x500 Layout](https://github.com/txoof/epdlib/blob/master/docs/weather_5x5.png)<br/> 500x500 Layout| ![300x200 Layout](https://github.com/txoof/epdlib/blob/master/docs/weather_3x2.png) <br/> 300x200 Layout|

### 


 
 <img src=https://github.com/txoof/audioSensor/blob/master/irBlaster.jpg alt="Audio Sensor" width=400 /></br>Audio Sensor
| NPR2Podcast | epdlib          | querylms     |
