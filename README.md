## ShareX Custom Uploader PHP File ![php](https://img.shields.io/badge/php-hypertext%20preprocessor-blueviolet?style=flat-square&logo=php&logoColor=white)
In this repository, you will find a single PHP file that you need to customize in order to set up a custom uploader properly.

## Requirements
 1. A text editor such as VSCode, Sublime, or Notepad++. Regular Notepad is not the tool for this job.
 2. A web host that does not block JavaScript or check for it.
 3. ShareX Client.

## Usage
This section will be formatted in a step by step process

 1. Download the "up.php" file from this repository and extract it out of the zip file
 2. Open the files in your text editor and you should see this: ![up.php file](https://i.imgur.com/oO3rYlk.png)
3. Please direct your attention to lines 2 through 5!
![Lines 2-5](https://i.imgur.com/fYWNT5R.png)
4. On "$secret_key" change the value to a secure password that you'd like to use, it can also be random letters and numbers, as long as you can copy and paste.
5. On "$sharexdir" you can leave this value blank.
6. On "domain_url" change the value to the website URL where you plan on storing the up.php file.
7. On "$lengthofstring" you can change the value if you want to but it is not required.
8. After you edit these values, save and close this file.
9. Next, put the file on your website using the same URL that you put on the "&domain_url" value.
10. Open up ShareX and go to Custom Uploader settings
11. Under "Uploaders" click add
12. Set the name of the uploader to whatever you like, I called mine cdn
13. Be sure that the request type is set to POST
14. Set the Request URL to the web address where your up.php file is stored
15. Set the file form name to "sharex"
16. Add a new argument named "secret" and set the value to the secret key you have set in the up.php file
17. When you're finished, your configuration should look like this:
![ShareX custom uploader configuration](https://i.imgur.com/odNOnS1.png)
18. Configuration is finished! Make sure you have ShareX set to use this custom uploader and it should work. 

## Questions
If you have any questions, feel free to email me at banko.production.network@gmail.com or create a new issue on this repository.
