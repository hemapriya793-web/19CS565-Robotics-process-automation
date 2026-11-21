## NAME: Hemapriya.s
## REG NO: 212225240051
## AIM:
To create a workflow in UiPath Studio that displays a welcome message using IF Condition and Switch Case activities.
SOFTWARE REQUIRED:
- UiPath Studio
- Windows Operating System
## ALGORITHM:
Step 1:
Launch UiPath Studio from the desktop or Start menu.
Step 2:
Click on New Project → Process.
Step 3:
In the project creation dialog box:
- Enter the process name as WelcomeMessage.
- Set the project location.
- Click Create.
Step 4:
Once the project opens, double-click Main.xaml to open the main workflow.
Step 5:
In the Activities panel, search for Input Dialog.
Step 6:
Drag and drop the Input Dialog activity into the design panel.
Step 7:
Enter the following details:
- Title: Welcome
- Label: Enter your name
- Result: Create a variable named userName.
Step 8:
Search for the If activity and drag it into the design panel.
Step 9:
Enter the condition:
userName <> ""

Step 10:
In the Then section, add a Message Box activity and enter:
"Welcome " + userName

Step 11:
In the Else section, add a Message Box activity and enter:
"Please enter your name"

Step 12:
Search for the Switch activity and drag it into the design panel.
Step 13:
Set the TypeArgument as String and enter:
userName

Step 14:
Add the following cases:
- Case "Hari": Display "Welcome Hari!"
- Case "Priya": Display "Welcome Priya!"
- Default: Display "Welcome User!"
Step 15:
Save the workflow using Ctrl + S.
Step 16:
Click the Run button to execute the workflow.
## PROCEDURE:
1. Open UiPath Studio.
2. Create a new Process project.
3. Name the project WelcomeMessage.
4. Open the Main.xaml file.
5. Add an Input Dialog activity to get the user's name.
6. Add an If activity to check whether the name is empty.
7. Display a welcome message if the name is entered.
8. Display an error message if the name is empty.
9. Add a Switch activity to check the entered name.
10. Add different cases for different names.
11. Save the workflow.
12. Click Run to execute the workflow.
## WORKFLOW:
The workflow uses Input Dialog, If Condition and Switch Case activities to display the welcome message.
             START
                |
                v
          Input Dialog
                |
                v
          IF Condition
                |
          +-----+-----+
          |           |
        TRUE         FALSE
          |           |
          v           v
    Welcome       Please Enter
    Message        Your Name
          |
          v
       Switch Case
          |
     +----+-----+
     |    |     |
   Hari Priya Default
     |    |     |
     v    v     v
  Welcome Welcome Welcome
   Hari   Priya   User
     |    |     |
     +----+-----+
          |
          v
          END

## OUTPUT SCREENSHOTS:

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/cb51a37f-9f6f-4d1d-86e1-739fe2a7b707" />

## RESULT:
Thus, the Welcome Message workflow was successfully created and executed in UiPath Studio using If Condition and Switch Case activities to display different welcome messages based on the user's input.
