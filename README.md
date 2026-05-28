# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
**Check file type**
```bash
file image.jpg
```
or view magic bytes:
```
xxd image.jpg | head
```

<img width="711" height="321" alt="image" src="https://github.com/user-attachments/assets/e737356a-670c-43c2-9cc8-eb33f06cf364" />


**Run StegExpose**
```bash
java -jar StegExpose.jar suspect.jpg
```
instead of StegExpose an alternative tool binwalk is used
```
binwalk wallpaper.jpg
```
<img width="748" height="135" alt="image" src="https://github.com/user-attachments/assets/7b754962-e0e1-4bbb-8040-5b8e7eb74d6a" />


## OUTPUT:

List of Images with Steganography Detection Scores and File Signature Details

<img width="822" height="245" alt="image" src="https://github.com/user-attachments/assets/6bf48293-77d9-42f6-beb5-9c193586979f" />



## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
