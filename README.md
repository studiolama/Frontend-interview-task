# React Interview project
# Problem statement
## _React.js, Frontend interview coding task_

Setup a new React Application.
Note : - You are free to use any CSS library or framework

Check figma file for better understanding of task and exact requirements
figma link : [https://www.figma.com/file/OahbXfHUfIM2Fc6B8Yeg3t/Internship-task?node-id=0%3A1&t=Jsh96WYtr7PKQx5k-1]



## Features
- Create a functional card component which has a multistep form
- There will be 4 steps of this form with proper validation

## Step-1
- First step will have user basic info input fields (you should use validations for each input field like: formik and yup validation) - you are free to use any validation library of your choice. 
 
**Validations for first step**
| Input Field | Validations |
| ------ | ------ |
Name | min 3 char is required and max 20 char is allowed and only space is not allowed|
|DOB | except current and future dates  allow all previous dates.|
|Radio button | Default is set to false.  Note : If yes then display another input field to ask for born in week(it should only allow number between 20 - 36)|
Child weight | optional |
Child height | optional |
Email | must be a valid email address |
Phone | must be a valid phone number|

- After successful validation enable the next button and save the complete object into the localstorage and also move the progress indicator to second step.

## Step-2
- In the second step display list of options with data as mentioned in the figma (json object is available in the constants folder refer to it and check figma link for design reference).
- It should have multiple select option i.e user should be able to select one or more options and each card should be toggleable(select and deselect).
- Store the selected options in the array of objects format in state using useState hook.
- Atleast one option is mandatory to proceed further otherwise disabled the next button but user should be able to move back to previous step as shown in figma there is back button on the top of the card.
- After selection display subcategory for each selected options one by one (subcategory data is available in the constants folder).
- Again user must be able to select/deselect any subcategory options and user should be able to select one or more options but atleast one option is mandatory
- Note : Make sure subcategory should be handled separately within second step. (Main progress steps should be at 2nd while category and subcategory selection).
- When user is in second step then back button on the top should work accordingly
   for example : If user has selected three category and user is in 2nd subcategory options list and if user clicks on back button then it should take the user back to previous subcategory options list not the previous step.
- After successful validation store all the data in the localstorage and allow next button and move the progress indicator to the 3rd step.

## Step-3
- In 3rd step display textarea where user can explain problems (it is optional field)
- If user entered any information and store it in state and onClick next button store the information in the local storage.
- Move the progress indicator to the 4th step.

## Step-4
- In the 4th step take basic information from the user using date and time selector/picker  and onClick Submit display all information in the final screen.
**Validations for 4th step**

| Input Field | Validations |
| ------ | ------ |
|Time and date | must be future date disabled all current and previous date |
|Slot | is toggleable any one is required |
|Call type | is optional but pre-select any one option |

## Display data
- Display are the information in the new page that you have stored in local storage in each step.

**Host it on any free server or send complete code in the github repo**


**Happy coding** 
If you did not able to complete or having problem in understanding the problem statement ?. Send your query at : 
hello@studiolama.design


 
