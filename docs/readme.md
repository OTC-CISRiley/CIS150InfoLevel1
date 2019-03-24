# Hello!

## Welcome to the TFS Treasure Hunt
The payload is stashed in GitHub, and must be properly stored in TFS.

## TFS Quick Reference
TFS is pretty simple to use, but you may need to refer to this Quick Reference while you learn.

[TFS Quick Reference - Connect to TFS](ConnecttoTFS.pdf)

## Begin Level 1
1.	Connect to tfs
2.	Create a new project – check the add to source control check box
- the check box adds the project to tfs control as the project is created
- you can use the file menu to add the project to source control at a later time

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
- this project uses an array to save web url's
- use your desk checking skills to see if you can determine what string is saved in each array entry
- run the debugger to validate your expected array contents
4.	Verify the tfs checkin using the source control explorer in Team explorer
5.	Raise your hand to show the instructor your valid tfs checkin (you will receive level 2 info)
 
6.	Log off the computer
7.	Log onto a different computer before beginning the next level.

![TFS Treasure](qr-treasure.png)
