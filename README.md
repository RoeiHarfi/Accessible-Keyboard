# LIAM keyboard

<img align="right" style="width:100px; height:auto;" src="https://github.com/user-attachments/assets/63151943-57ae-41cb-a613-d058679d0e68">

### Accessible Keyboard Project

A final college project written in Swift using Xcode and SwiftData.<br>
Description: an iPad app application featuring a specialized keyboard designed to teach reading Hebrew using the LIAM (ליע"ם) method, tailored for children and adults with special needs and communication difficulties.<br>
Includes real-time auditory feedback, image-based writing exercises, and progress tracking capabilities.

<table align="center">
 <thead>
   <tr>
      <td colspan="2" align="center">Collaborators</td>
   </tr>
   </thead>
   <tbody>
    <tr>
      <td align="center"><a href="https://github.com/ElenaChes">@ElenaChes</a></td>
      <td align="center"><a href="https://github.com/RoeiHarfi">@RoeiHarfi</a></td>
      </tr>
      <td>
         <a href="https://github.com/ElenaChes"><img src="https://github.com/ElenaChes.png?size=115" width=100 /></a>
      </td>
      <td>
         <a href="https://github.com/RoeiHarfi"><img src="https://github.com/RoeiHarfi.png?size=115" width=100 /></a>
      </td>
   </tr>
   </tbody>
</table>

<details>
  <summary><h3>Content</h3></summary>

- [Installation](#installation)
- [Screens](#screens)
  - [Main Screen](#main-screen)
  - [Secondary Screen](#secondary-screen)
  - [Teacher Screen](#teacher-screen)
  - [Statistics Screen](#statistics-screen)
  - [Images Screen](#images-screen)
- [Usage](#usage)

</details>
<hr>

# Installation

1. Open the project using Xcode 15 or higher.
2. Install the app on an iPad.

> [!IMPORTANT]
> The app was developed for iPadOS 17.

# Screens

## Main Screen

<img align="right" style="width:300px; height:auto;" src="https://github.com/user-attachments/assets/0a3a266c-18c0-4f81-a8f4-cbf8e9302a3a">

The first screen of the app, here a student can:

- Swap between boards using the `yellow` vowel (nikkud) keys.
- Type using the `white` and `green` letter keys from the selected board, there will be auditory feedback for the user to make sure they typed the letter they wanted.
- Add space (`רווח`), delete the last letter (`מחק תו`) or word (`מחק מילה`).
- Tap the `speaker` icon at the top left corner to hear what was typed into the text line.
- Go to the secondary "settings" screen using the `blue` gears icon.

> [!IMPORTANT]
> Grey vowel keys indicate disabled boards. A teacher user can unlock boards for student users.

## Secondary Screen

<img align="right" style="width:300px; height:auto;" src="https://github.com/user-attachments/assets/a8500cd1-a638-41db-a504-74e287260400">

Also considered the settings screen of the student user, here a user can:

- Go to the main screen using the `blue` arrow icon.
- Swap between `color themes` from the 4 options at the bottom of the screen.

### Log in as another student user:

1. Tap the `dropdown` at the top right corner and select a name.<br>
   No password will be requested on login because no personal data gets saved on users.

> [!NOTE]
> This feature lets multiple students to use the same iPad and still have separate progress tracking for each.

> [!IMPORTANT]
> A teacher user can add, edit and remove student users from the users list.

### Enter image mode:

1. Go through the available images per board using the `yellow` vowel keys and the `arrow` keys.
2. Tap an image to select it.
3. The app will redirect to the main screen in image mode.
4. In this mode a student can:
   - Tap the `image icon` to see a larger preview of it, tap on it again to close it.
   - Type the description of what's in the image.
   - Click the `green` checkmark to submit what they wrote.

<p align="center">
 <img style="width:400px; height:auto;" src="https://github.com/user-attachments/assets/375484aa-f958-40b7-b4ad-6dddf06c592c">
</p>

The app calculates typos (compared to what's written in the image's description) and adds the student's progress to their statistics.

> [!Tip]
> To exit image mode without altering the statistics make sure the text line is empty.

> [!Note]
> The app has a built in database of images with set descriptions, but a teacher user can add additional images with custom descriptions.

### Login as teacher to gain access to the teacher settings screens:

1. Tap the login button at the left top corner (`כניסת מורה`).
2. Input the default teacher password `teacher123`.
3. Tap the login button again.
4. The app will then redirect to the teacher screen.

> [!Note]
> The app doesn't store any personal information, so the teacher login needing a password is only to ensure that student users can't get into them on accident and "get lost" in the app.

## Teacher Screen

<img align="right" style="width:300px; height:auto;" src="https://github.com/user-attachments/assets/b4bba38b-faec-473a-9ae1-aeeac49d182d">

The teacher's main screen, accessible via loggin in as a teacher. The screen has a few options:

- Go to the secondary screen using the `blue` arrow icon.
- Navigating to the statistics screen (`סטטיסטיקת תלמידים`).
- Navigating to the images screen (`הוספת תמונות`).

### The images (מאגר תמונות) section:

1. Go through boards using the `dropdown` and `arrows`.
2. Tap on images to see their descriptions.

> [!Note]
> This is the only place where a user can see the description of the built in images.

### The students (תלמידים) section:

- Adding a user:
  1. Select the new user (`תלמיד חדש`) option in the dropdown.
  2. Type the name you want the user to have in the name field.
  3. Tap the save button (`שמור`).
- Renaming a user:
  1. Select a student from the `dropdown`.
  2. Type the name you want the user to have in the name field.
  3. Tap the update button (`עדכן`).
- Deleting a user:
  1. Select a student from the `dropdown`.
  2. Tap the delete button (`מחק`).

### The boards (פתיחת לוחות) section:

- Select a student from the `dropdown`.
- Tap the sliders for the boards you want to lock or unlock for that user.

> [!Note]
> The first board can't be locked.

## Statistics Screen

<img align="right" style="width:300px; height:auto;" src="https://github.com/user-attachments/assets/fc94241c-c20e-45a1-ab49-432cb1c20d2b">

- Go to the teacher screen using the `blue` arrow icon.
- Select a student from the `dropdown`.

### View the progress of the student in a table:

Scroll to view activity per date.

- Total words (`סה"כ מילים`):
  - The amount of words the student typed in a day.
  - Essentially the amount of times the green checkmark in "image mode" was tapped.
- Correct words (`מילים נכונות`):
  - The amount of words the student typed correctly in a day.
  - Words that were typed with no typos are considered correct words.
- Total letters (`סה"כ אותיות`):
  - The amount of letters in the words the student typed in a day.
  - A sum of the letters of all the images that got selected in "image mode" and submitted.
- Typos (`שגיאות כתיב`):
  - The amount of typos the student made in a day.
  - A sum of the letters the student typed that didn't fit the image's description.

### View the progress of the student in graphs:

- Typos/Total letters percentage per day (`שגיאות כתיב מתוך סה"כ`).
- Correct words/Total words percentage per day (`מילים נכונות מתוך סה"כ`).

## Images Screen

<img align="right" style="width:300px; height:auto;" src="https://github.com/user-attachments/assets/64085977-4393-4c74-a53c-48a8f9ac5590">

- Go to the teacher screen using the `blue` arrow icon.
- Updating an image:
  1. Go through boards using the `dropdown` and `arrows`.
  2. Tap the image you'd like to edit.
  3. Type the description you want the image to have in the description field.
  4. Tap the save button (`שמור`).
- Adding an image:
  1. Tap the new image (`הוסף תמונה חדשה`) button at the bottom of the screen.
  2. Select the image you'd like to add.
  3. Type the description you want the image to have in the description field.
  4. Tap the save button (`שמור`).
  - To cancel adding an image tap the delete button (`מחק`).
- Deleting an image:
  1. Go through boards using the `dropdown` and `arrows`.
  2. Tap the image you'd like to remove.
  3. Tap the delete button (`מחק`).

> [!NOTE]
> Built in images don't appear on this screen and can't be removed from the app.

> [!IMPORTANT]
> The description of an image needs to have proper spelling and nikkud, as it's what the app compares to in "image mode" to check if the student spelled the image description correctly.

# Usage

1. If more than one student uses the app on this iPad make sure the student selects their name in the secondary screen.
2. Teach the student as you would using the LIAM method, ask them about the sounds, let them type, and use the "image mode" when working with images.
3. Unlock more boards in the teacher screen as the student progresses and check their progress in the statistics page.
4. Add new student users and new images as necessary.

> [!TIP]
> If during teaching you'd like to be able to type a letter without it making a sound just mute the iPad output.

> [!NOTE]
> The app is fully local, it uses no external storage and doesn't need an internet connection.
