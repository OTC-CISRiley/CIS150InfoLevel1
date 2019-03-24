# Hello!
[TFS Quick Reference - Connect to TFS](ConnecttoTFS.pdf)

1.	Connect to tfs
2.	Create a new project – check the add to source control box

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



3.	Code the project and check it in and commit to tfs
4.	Verify the tfs checkin using the source control explorer in Team explorer
5.	Raise your hand to show the instructor your valid tfs checkin
a.	You will receive 
6.	Log off the computer
7.	Log onto a different computer before beginning the next level.
