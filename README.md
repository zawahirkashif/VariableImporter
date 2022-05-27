# What is Variable Importer?

The Variable Importer script enables you to automate many of the previously annoying aspects of the usual methods of importing variable data into Illustrator.
The top issues resolved with the script are:
- XML is generated automatically by the script, allowing you to import a plain old csv file just like InDesign.
- Filepath to images automatically linked by the script. No more hunting down the correct syntax to input a filepath into your csv.
- Variables can be “auto bound” to objects, sparing you yet another annoying step of manual binding
- You can customize Dataset names at import time.
There are many more little niceties within the script, so let’s go ahead and take a look.

## Get The Variable Importer Script

![Download](https://cdn.loom.com/images/originals/970bed8321424ee2a399626e8735f660.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jZG4ubG9vbS5jb20vaW1hZ2VzL29yaWdpbmFscy85NzBiZWQ4MzIxNDI0ZWUyYTM5OTYyNmU4NzM1ZjY2MC5qcGciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE2NTM3MDQzNjl9fX1dfQ__&Key-Pair-Id=APKAJQIC5BGSW7XXK7FQ&Signature=nL-VDQopLaBjfxk-MOauMVg1tyCjf4R5NLG2wcOTKJBb9u8RD344JFDNLDmDdWVpJLgKGJA0HXB2%7EvgTm6-3zEYPqfHYy0Ur2E7%7EpBy85fNA%7EB1yQcdq33T1uclfn3tZnV1X2dp3vb7BnqXYkta4sk3yX0-VmrFme7GQB9wZgfAoVMPuXTCTSFpXBYF0eWcnPnh8zjzkHgt%7ELW7RGWrMpshr1JibU0rY2f0fSgbvj4NME%7EjLA76giWrXcKNb2HM-KqlptWirvQI23rNB0FD1qDV6aTY7Hdlbhs61EEmY4L5IuWowCiY9UJumC%7ERtvZZaX8zEjn4lMwEQQrQ81sUq8A__)


First we have to get the script installed in Illustrator. To do this, first go to the [Variable Importer](https://github.com/zawahirkashif/VariableImporter).

Once you get there, click on “VariableImporter.jsx”, then click the “Raw” button (shown in screenshot above). This will bring up a page that contains the raw code of the script. From here just “Save as…” from your browser to download (don’t just right-click the “VariableImporter.jsx” and save, because that way will introduce errors into the script – make sure to only save the “raw” code).

- Now drag and drop the script in your illustrator.
#### Variable Importer Dialog Box
![](https://cdn.loom.com/images/originals/2ae4802d23a9443eb9bbf5bd4ff3854c.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jZG4ubG9vbS5jb20vaW1hZ2VzL29yaWdpbmFscy8yYWU0ODAyZDIzYTk0NDNlYjliYmY1YmQ0ZmYzODU0Yy5qcGciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE2NTM3MDU1Nzl9fX1dfQ__&Key-Pair-Id=APKAJQIC5BGSW7XXK7FQ&Signature=eoK9luv8U86sDXZrNCZ5sYiUUyjjqEhBD%7E8pWCV9Wt9w6ekRqCNPuk3gFDalKrre1gAI%7EDjxM7tBWNNtkoRsAEf0GvqerVBFHhEhbbAU6iKAxss1y%7EjhhgzNp02QG6tTeaxtUgcI%7Euf916zj4qeJm1%7EQ04hC%7ECyYTYRN9V30AdoJsiFXulLEqNXOtTiaVAU15JCX%7EjW6IgZ2hy6DUlGCAXmyl4%7EsrLa6opzV65lkEqN%7E2T1GCY-xUk7qY0lcXlnNSHpV6R0yCvw-qkzPe6x-aSQTksO0lq0GziL5uxeNOAQ2TXY-syfoc6JoCZc3gW6QSb6cxEliII71AHTkbE9vtg__)

- Create a .csv file you want to insert in your illustrator template
#### Test Data CSV file
![](https://cdn.loom.com/images/originals/376d699856a440fbafa108059f606369.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jZG4ubG9vbS5jb20vaW1hZ2VzL29yaWdpbmFscy8zNzZkNjk5ODU2YTQ0MGZiYWZhMTA4MDU5ZjYwNjM2OS5qcGciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE2NTM3MDU4MzF9fX1dfQ__&Key-Pair-Id=APKAJQIC5BGSW7XXK7FQ&Signature=R1Nw9x9V3lbIl6L6k6t30%7EuSbdDXL%7EUHG4GwYuyzc9v%7EP0glHxk6kcTDpmr2l1fxoaOcKTSPKtGTujPOTK-QbIwQj0MUotADZjFIZA7XRiZO4aKehbPYtwqWpcMgyTMPUYCjZ-MR0h2zrwrv11BFGYQZFTb0EQRhxhjlRMGkaCuwa4T7p%7EEkKh-MUqxZX68LgL1XZowSeAO-nZ3EK2359hf0B4uRno-puYbw81MYV4wdOCSdgDpsIPwU2Jnt28F9QzPvNrWVAoGjvqbOcl237Kzi5EYcYPxXiH2NfI14lhb1%7EntR7H2kVqtYC7FpORLYV-EM13bNFIcstk3LUte3mA__)

- Choose the .csv file 
#### Select Test Data CSV file
![image](https://user-images.githubusercontent.com/49830314/170618857-322a5564-02f7-4b45-aace-b77d8734d16f.png)

- Click on option in the Variable Import dialogue 
#### Import Variables
![image](https://user-images.githubusercontent.com/49830314/170618960-7a2f84f5-3a67-4fa0-b73c-434f83a2e183.png)
- Click on import variable
- Goto windows > variables in Adobe Illustrator.
#### Variable Window In Illustrator
![image](https://user-images.githubusercontent.com/49830314/170619269-2ff34fe6-9a5d-469f-8c21-af734786164a.png)

- Now we will bind the the variables
#### Binding Variables
https://user-images.githubusercontent.com/49830314/170620466-15ecebd9-f8a8-4571-83eb-9849dd823ef9.mp4

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch 
3. Commit your Changes 
4. Push to the Branch 
5. Open a Pull Request


## License

Distributed under the MIT License. See `LICENSE.txt` for more information.


## Contact

Your Name - [@SMZawahir1](https://twitter.com/SMZawahir1) - zawahirkashif@gmail.com

Project Link: [https://github.com/zawahirkashif/VariableImporter](https://github.com/zawahirkashif/VariableImporter)








