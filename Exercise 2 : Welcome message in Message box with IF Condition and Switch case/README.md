## Exercise 2 : Welcome message in Message box with IF Condition and Switch case

## NAME: Hema priya.S

## REGISTER NUMBER: 212225240051

## AIM

To create a workflow in UiPath Studio to get the user's name as input and display a welcome message using IF Condition and Switch Case activities.

## SOFTWARE REQUIRED:

Software Used: UiPath Studio

## ALGORITHM

## Part A: Using IF Condition

Step 1:
Launch UiPath Studio from the desktop or Start menu.

Step 2:
Click on New Project → Process.

Step 3:
In the project creation dialog box:

Enter the process name as WelcomeMessageIf.

Set the project location (e.g., Documents\UiPathProjects).

Click Create.

Step 4:
Once the project opens, double-click Main.xaml to open the main workflow.

Step 5:
Open the Variables panel at the bottom of UiPath Studio.

Step 6:
In the Activities panel, search for Input Dialog and drag it onto the design panel.

Step 7:
Set the Input Dialog properties:

Title: Enter Name

Label: What is your name?

Output variable: userName (String).

Step 8:
Below the Input Dialog, search for the If activity and drag it onto the design panel.

Step 9:
Set the Condition as:

userName.ToUpper = "RAM"

Step 10:
In the Then section, add a Message Box activity and enter:

"Welcome Mr. Ramachandran"

Step 11:
In the Else section, add another Message Box activity and enter:

"Welcome " + userName

Step 12:
Save the workflow using Ctrl + S.

Step 13:
Click the Run button (green play icon) at the top of UiPath Studio.

Step 14:
Enter different names to check the welcome messages.

## PROGRAM WORKFLOW:

## Part A: Using IF Condition

The workflow uses an Input Dialog activity to get the user's name. The IF Condition checks whether the entered name is RAM. If true, it displays "Welcome Mr. Ramachandran"; otherwise, it displays "Welcome" followed by the given name.
```

          START
             |
             v
        Input Dialog
        (Enter Name)
             |
             v
       IF Condition
    userName.ToUpper = "RAM"
          /       \
       TRUE       FALSE
        |           |
        v           v
   Message Box  Message Box
   "Welcome Mr.  "Welcome " +
   Ramachandran" userName
        |           |
        v           v
           END
```

## UiPath Workflow.

<img width="546" height="537" alt="image" src="https://github.com/user-attachments/assets/5d02d574-6132-4f43-8025-03a1ba301359" />

<img width="535" height="395" alt="image" src="https://github.com/user-attachments/assets/c712aa7e-bf9e-4b14-a596-ab19c047e855" />


## OUTPUT

## Execution Output:

<img width="355" height="197" alt="image" src="https://github.com/user-attachments/assets/ecdc63c0-7896-4d00-a097-7139b447d6ca" />

<img width="217" height="162" alt="image" src="https://github.com/user-attachments/assets/4c502be6-fbe8-4108-88a4-0c8da6b6992e" />


## Part B: Using Switch Case
## AIM

To create a workflow in UiPath Studio using the Switch Case activity to display different welcome messages based on the user's input.

## ALGORITHM

Step 1:
Launch UiPath Studio from the desktop or Start menu.

Step 2:
Click on New Project → Process.

Step 3:
In the project creation dialog box:

Create a new project or use the existing project.

Set the project name as WelcomeMessageSwitch.

Choose a save location and click Create.

Step 4:
Once the project opens, double-click Main.xaml to open the main workflow.

Step 5:
From the Activities panel, search for Input Dialog and drag it onto the design panel.

Step 6:
Set the Input Dialog properties:

Title: Enter Name

Label: What is your name?

Output variable: userName (String).

Step 7:
After the Input Dialog activity, search for Switch and drag it onto the design panel.

Step 8:
In the Switch properties, set the Expression as:

userName.ToUpper

Set the TypeArgument as String.

Step 9:
Create the following cases in the Switch activity:

Case ALICE → Add Message Box: "Welcome Alice! Have a great day."

Case BOB → Add Message Box: "Hi Bob! Welcome back."

Case CHARLIE → Add Message Box: "Hello Charlie, glad to see you!"

Step 10:
In the Default case, add a Message Box and enter:

"Hello " + userName + ", Welcome!"

Step 11:
Save the workflow using Ctrl + S.

Step 12:
Click the Run button (green play icon) at the top of UiPath Studio.

Step 13:
Enter different names and observe the corresponding welcome messages.

## PROGRAM WORKFLOW:

The workflow uses Input Dialog to get the user's name and Switch Case to display different welcome messages for different inputs.
```
             START
                |
                v
           Input Dialog
           (Enter Name)
                |
                v
           Switch Case
         userName.ToUpper
                |
       +--------+--------+
       |        |        |
       v        v        v
     ALICE     BOB    CHARLIE
       |        |        |
       v        v        v
    Message  Message  Message
      Box      Box      Box
       |        |        |
       +--------+--------+
                |
                v
             DEFAULT
                |
                v
            Message Box
                |
                v
               END
```
## UiPath Workflow:

<img width="693" height="537" alt="image" src="https://github.com/user-attachments/assets/ba57d6f2-7c86-4a96-be49-2f53292030b4" />

<img width="602" height="593" alt="image" src="https://github.com/user-attachments/assets/8fecd60a-2fce-4f08-b735-c9d1f31a6918" />


## OUTPUT

## Execution Output:

<img width="345" height="188" alt="image" src="https://github.com/user-attachments/assets/d2d0f05e-dd10-4824-865e-cff7cd83d75c" />

<img width="217" height="162" alt="image" src="https://github.com/user-attachments/assets/30678d16-4ec2-4fb7-9abe-51fd9a5adeb0" />


## RESULT

Thus, the Welcome Message workflow was successfully created and executed in UiPath Studio using IF Condition and Switch Case activities. The appropriate welcome messages were displayed successfully based on the user's input.

