# EXPERIMENT 1 : HELLO WORLD - DISPLAY A MESSAGE BOX
## NAME : Hema priya.s
## REG NO : 212225240051
## AIM:

To create a workflow in UiPath Studio that displays a "Hello World" message box.

## SOFTWARE REQUIRED:

- UiPath Studio
- Windows Operating System

## ALGORITHM:

### Step 1:
Launch UiPath Studio from the desktop or Start menu.

### Step 2:
Click on **New Project → Process**.

### Step 3:
In the project creation dialog box:
- Enter the process name as `HelloWorld`.
- Set the project location (e.g., `Documents\UiPathProjects`).
- Click **Create**.

### Step 4:
Once the project opens, double-click `Main.xaml` to open the main workflow.

### Step 5:
In the Activities panel on the left side, search for **Message Box**.

### Step 6:
Drag and drop the Message Box activity onto the design panel.

### Step 7:
Click inside the Message field of the Message Box activity.

### Step 8:
Enter the following text in the Message field:

```text
"Hello World"
```

### Step 9:
Save the workflow using `Ctrl + S` or select **File → Save**.

### Step 10:
Click the **Run** button (green play icon) at the top of UiPath Studio.

## PROCEDURE:

1. Open UiPath Studio.
2. Create a new Process project.
3. Name the project `HelloWorld` and select the required location.
4. Open the `Main.xaml` file.
5. Search for the Message Box activity in the Activities panel.
6. Drag the Message Box activity into the design panel.
7. Enter `"Hello World"` in the Message field.
8. Save the workflow.
9. Click the Run button to execute the workflow.

## WORKFLOW:

The workflow uses a Message Box activity to display the required message.

```text
       START
          |
          v
   Message Box Activity
          |
          v
 Display "Hello World"
          |
          v
        END
```

# OUTPUT SCREENSHOTS:

## 1. UiPath Workflow.
<img width="688" height="323" alt="image" src="https://github.com/user-attachments/assets/5581dd6a-68c9-424f-8ca0-1594d5cce33a" />

## 2. Execution Output.
<img width="238" height="242" alt="image" src="https://github.com/user-attachments/assets/b631f99f-ed5b-4dab-bfc7-53f0d2ad6059" />


# RESULT:
Thus, the Hello World workflow was successfully created and executed in UiPath Studio using the Message Box activity, and the message "Hello World" was displayed successfully.
