# Hello!

## Welcome to the TFS Treasure Hunt
The payload is stashed in GitHub, and must be properly stored in TFS.

## TFS Treasure Map (Quick Reference)
TFS is pretty simple to use, but you may need to refer to this Quick Reference while you learn.

[TFS Quick Reference - Connect to TFS](ConnecttoTFS.pdf)

## Begin Level 1
1.	Open Visual Studio
2.	Connect to tfs using Team Explorer in Visual Studio
3.	Create a new Visual Studio project – check the add to source control check box
- the check box adds the project to tfs control as the project is created
- you can also use the file menu to add the project to source control at a later time

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



3.	Code the project and check it in to tfs
- this project uses an array to save web url's, giving you a bit of a preview to our array lesson!
- use your desk checking skills to see if you can determine what string is saved in each array entry
- run the debugger to validate your expected array contents
4.	Verify the tfs checkin using the source control explorer in Team explorer
5.	Log off the computer
6.	To verify that you can connect to TFS again, log onto a different computer or restart your computer before using the next clue

![TFS Treasure](qrcd-treasure.png)


The clue is in a QR Code. A QR Code is a great way to stash a URL or other data. I used a QR code generator to create this, and you can use a QR code reader to read it. 
