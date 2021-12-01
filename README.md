# Science Fair 2021 - Predicting Human Behavior Using Deep Learning Market Prediction
This repository includes much of the code and information from the 2021 Jasper High School Science Fair competition of Khosraw Azizi's project. 

**Dataset Used:** https://drive.google.com/file/d/17QBUbCeGAtktoaG1PTZkWDUBQkh3PW9u/view?usp=sharing

**Original Dataset:** https://www.kaggle.com/mczielinski/bitcoin-historical-data

##
- A laptop:
  - Processor - Intel(R) Pentium CPU 4405U @ 2.10GHz (2 Cores | 4 Threads)
  - Installed RAM - 4.00GB (3.86GB Usable)
  - 500GiB HDD
  - System Type: 64-Bit, x64-based processor
  - OS: Linux Kernel 5.14.11-Zen of GNU/Linux (Can be Windows)
  - Distribution: Archcraft
  - Has Access to a Stable WIFI Connection
  - Contains a web browser (Vivaldi)
- Email Account (khosraw.azizi@gmail.com | Recommended no school, work, or organization email addresses)
- Website - colab.research.google.com, https://github.com/Khosraw/Science-Fair-2021---Predicting-Human-Behavior-Using-Deep-Learning-Market-Prediction

## Procedure
1. Plug in the laptop's charging cord into a power socket and the other end of the power cord into the laptop's charging port.
2. Press the power button on the computer.
3. If the material involves Windows or if there is no duel booting (running multiple operating systems at the same time), skip to step 4. Otherwise, use the arrow keys to navigate to the proper operating system and press the enter key on the keyboard.
4. If prompted to enter a password to log in, enter the password using the keyboard.
5. Once logged in, if on Windows, press the Windows/Super key and type the name of the browser that will be used. If on Linux with Archcraft, press the Windows/Super key and type the exact name of the browser, and then press enter to open it. If using any other Linux distribution, the process will always vary depending on the distribution.
6. If on Windows, check the bottom right corner of the screen to see if the WIFI symbol has full or partially full white bars. If yes, skip to step 7. If no, click on the WIFI symbol to open up the WIFI menu, and then click the WIFI connection chosen to connect to, and if required a passcode, enter the passcode using the keyboard and press the enter key. If on Archcraft Linux, check the top bar for the WIFI symbol and see if the WIFI symbol is crossed out and/or is red. If no, skip to step 7. If yes, press the Windows/Super key with the N key to open up the WIFI menu. Once open in the menu, use the up and down arrow keys to navigate up and down the connections list, or use left and right to go through the different pages. If asked for a passcode, use the keyboard to enter it and press enter.
7. Once the browser is open, click on the top empty search bar.
8. Once the cursor in the search bar starts blinking, type in the following link into it using the keyboard, and then press enter: https://github.com/Khosraw/Science-Fair-2021---Predicting-Human-Behavior-Using-Deep-Learning-Market-Prediction
9. Once the page is fully loaded, see the box labeled at the top as "README.md", scroll down until the text labeled "Dataset Used:" can be seen, and middle-click on the link to the right of that text.
10. If the new tab cannot be seen on screen, see the top bar of the browser where tabs are listed and click on the one labeled with "output.csv". Otherwise, click on the button labeled "Download", and save the file to a location on the computer. 
11. Switch back to the tab with the GitHub page labeled with "Khosraw".
12. Look through the top box where files are listed, and click on the file labeled "SF_TF_BTC_Final.ipynb" on the left side of the box.
13. If the page is loaded to a website linked colab.research.google.com shown at the top of the browser (the address/search bar) and there is no button on the top right of the page labeled Sign In, skip to step 17. Otherwise, click on the Sign In button on the top right.
14. If the page contains an available list of accounts, click on the preferred account and skip to step 15. If not, click on the empty box for the emails and type in the full email address for the account, and then click on the button labeled Next. 
15. Click on the empty box for the password field and enter the password for the corresponding email address chosen previously, and click the button labeled Next.
16. If asked to use Two-Factor authentication, proceed with the preferred way to authenticate the account. Otherwise, skip to step 17.
17. Identify the top row of buttons in the Colab website labeled with File, Edit, View, Insert, Runtime, Tools, and Help.
18. Hover the mouse over the Runtime item in the top row and click on it.
19. Hover the mouse over the "Change runtime type" and click on it.
20. Once a box labeled "Notebook settings" appears, click on the dropdown menu below the label titled "Hardware accelerator", and click on the item labeled GPU. 
21. Once set, click on the button labeled "Save".
22. Identify the Folder/File icon on the left side of the page and hover the mouse over it to then click on the button.
23. Once the "Files" tab expands, click on the button with the file icon and an arrow pointing upwards inside the icon to upload a file. 
24. Navigate to the location where the previously downloaded "output.csv" is, and double click it to upload it to Colab.
25. If a window labeled with "Reminder, uploaded files will get deleted when this runtime is recycled." opens, click on the button labeled "OK". Otherwise, skip to step 26.
26. Click on the top row button labeled Runtime and click on the button labeled "Run all".
27. If a window titled "Warning: This notebook was not authored by Google." comes up, click on the button labeled "Run anyway" to proceed. Otherwise, skip to step 28.
28. Use the scroll wheel on a mouse or two fingers to scroll down the page until the output is visible with outputs such as "Epoch 1/100".
29. Observe the loss/mae (mean absolute error) of each epoch being displayed until the model stops training.
30. When a graph is displayed at the end of the output box, it means that the model is done training. Observe the graphs, along with the final training loss/mae at the last labeled epoch, and observe the final row of evaluation where the output states with "62/62" for the testing loss/mae. 
31. Using the previously observed testing loss/mae value, record that the final predictions for the trained model are on average loss/mae dollars off the true pseudo-future values (Ex: $26.96 off since the loss/mae value is 26.9553).


## Graphs

**Graph of Dataset:** 
![fab250fd-debc-43d0-8546-f3d2ca664513](https://user-images.githubusercontent.com/53713571/144168716-9edbbf5b-9ee8-40eb-9076-d8b20fe55605.png)

**Graphs of final product:**

![094acfd0-4f4d-4649-ae57-546c9e58f60c](https://user-images.githubusercontent.com/53713571/144160729-77b1a2b6-0da4-41a6-9be8-c01e491e5625.png)
![1d3ba0f7-b58a-4baf-a724-512456ed55e9](https://user-images.githubusercontent.com/53713571/144160884-67648d8c-00f7-4880-a3f5-51ecf46cfb2d.png)
![download (1)](https://user-images.githubusercontent.com/53713571/144160961-f70a41ce-7c7f-4a38-a6fb-670f412a033f.png)
![13e69281-c75e-45b2-a6df-7d1babfafc7c](https://user-images.githubusercontent.com/53713571/144160973-7c03528c-0672-47fc-a832-23cf44d9b8ed.png)
