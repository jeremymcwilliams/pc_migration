Code base for the Lewis & Clark Publications & Communications department's digital image library migration from Aperture to Omeka.

For a given export directory of images and metadata, the code does the following:

1) Creates Omeka-ready collection specific csv-files<br/>
2) Uses exiftool to gather metadata from images<br/>
3) Possibly FTPs images to appropriate spots<br/>


Uses the following:<br/>
-exiftool<br/>
-html5 boilerplate<br/>


Some Requirements:
1) Symbolic link to Desktop set in your local code directory
-this may require un-doing and re-doing the symbolic link on a local computer
-in terminal, navigate to /Library/WebServer/Documents/pubcom/ and do the following:<br/>
rm Desktop<br/>
ln -s /Users/{username}/Desktop Desktop<br/>
(replacing {username} with your real username)<br/>
<br/>
2) A writable directory on your Desktop called "OmekaCSVfiles"<br/>
<br/>
3) A writable directory on your Desktop called "converted"<br/>
