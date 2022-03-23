# Hello!

## Welcome to the TFS Treasure Hunt
The payload is stashed in GitHub, and must be properly stored in TFS.

## TFS Treasure Map (Quick Reference)
TFS is pretty simple to use, but you may need to refer to this Quick Reference while you learn. You should save it for future use.

[TFS Quick Reference - Connect to TFS](ConnecttoTFS.pdf)

## Create your TFS Project Folder on the TFS Server
1.      After creating your Folder, proceed with Clue 1
2.      This project can be used for all of your C# code, so you only need to do this once


## Begin Clue 1
1.	Open Visual Studio
2.	Choose Continue Without Code
3.	Connect to tfs using Team Explorer in Visual Studio
4.	Create a new Visual Studio project – note the project will be created in your Local Workspace
- Do use the local workspace for your project location
5.      On the File menu, choose Source Control, Add Solution to Source Control
- Save the solution in your TFS Project folder, created earlier

        static void Main(string[] args)
        {
        
            string sitePre = @"https://otc-cisriley.github.io/CIS1";
            int sizeOfArray = 0;
            string[] sites;

            // set up our number of sites array
            Write("\nHow many sites to load? ");
            while (int.TryParse(ReadLine(), out sizeOfArray) == false)
            {
                Write("\nHow many sites to load? ");
            }
            // allocate the array, based on the input
            sites = new string[sizeOfArray];

            // for loop to load the array with possible url's
            for (int i = 0; i < sizeOfArray; i++)
            {
                sites[i] = sitePre + i + @"0Info/";
            }
        }


6.	Code the project and check it in to tfs
- this project uses an array to save web url's
- use your desk checking skills to see if you can determine what string is saved in each array entry
- run the debugger to validate your expected array contents
7.	Verify the tfs checkin using the source control explorer in Team explorer and/or the TFS Web Portal
8.	Log off the computer
9.	To verify that you can connect to TFS again, log onto a different computer or restart your computer 


Time for the next clue

![TFS Treasure](qr-code-new.png)


The clue is in a QR Code. A QR Code is a great way to stash a URL or other data. I used a QR code generator to create this, and you can use a QR code reader to read it. Your phone's camera may have a built in QR code reader, or you may have to download an app.
