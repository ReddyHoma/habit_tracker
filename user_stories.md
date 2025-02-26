# User Stories for Habit Tracker App

## Login & Registration Page

### User Story 1: Account Registration
**Title:**  
_As a user, I want to register with my name, username, age, and country so that I can create an account and access the habit tracking features._

**Acceptance Criteria:**  
1. The user must enter their name, username, age, and country.  
2. A confirmation message appears upon successful registration.  
3. The system prevents duplicate usernames.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- The user credentials are removed from the browser cache after logging out.  

---

### User Story 2: Account Login
**Title:**  
_As a user, I want to log in using my username and password so that I can access my account and track my habits._  

**Acceptance Criteria:**  
1. The user must enter their correct username and password.  
2. An error message appears for incorrect credentials.  
3. A successful login redirects the user to the homepage.  

**Priority:** High  
**Story Points:** 2  

**Notes:**  
- Users can only log in using the default username and password.

---

### User Story 3: Error feedback on login
**Title:**
_As a user, I want to receive a message if I enter the wrong username or password so that I know my login attempt was unsuccessful._

**Acceptance Criteria:**
1. Display an error message if the user enters incorrect login details.  
2. Ensure failed login attempts do not reveal security-sensitive information.  
3. Provide an option to reset the password.

**Priority:** High  
**Story Points:** 2  
**Notes:**  
- Security constraints prevent credentials from being saved in the cache.  

---

## Homepage

### User Story 4: View Welcome Message
**Title:**  
_As a user, I want to see a personalized welcome message with my name on the homepage so that I feel recognized and can confirm I am logged into the correct account._  

**Acceptance Criteria:**  
1. Display a welcome message with the user’s name.  
2. Ensure the name updates dynamically if changed in the profile.  
3. Hide the message when the user logs out.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:** 
- The welcome message should be prominently displayed at the top of the homepage.  
- If the user does not have a name set, display a generic welcome message instead.  
- Ensure accessibility compliance by supporting screen readers for the message.

---

### User Story 5: Display Weekly Progress
**Title:**  
_As a user, I want to see my daily progress for each habit on the homepage so that I can easily monitor my progress._  

**Acceptance Criteria:**  
1. Show a summary of habits completed for each day of the week.  
2. Provide a visual indicator of progress (e.g., a progress bar).  
3. Ensure the data updates in real-time.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- The progress display should be visually distinct and easy to interpret at a glance.   

---

### User Story 6: View Completed Habits
**Title:**  
_As a user, I want to see a section for completed habits on the homepage so that I can track what I have already achieved._  

**Acceptance Criteria:**  
1. Display a separate section for completed habits.  
2. Allow users to filter completed habits by date.  
3. Ensure habits marked as completed are stored persistently.  

**Priority:** High  
**Story Points:** 2  
**Notes:**  
- Completed habits should be distinguishable from ongoing habits to avoid confusion.  

---

## Menu

### User Story 7: Access Menu Options
**Title:**  
_As a user, I want to access a menu with options for configuring my habits, viewing reports, editing my profile, and signing out so that I can easily navigate to different parts of the app._  

**Acceptance Criteria:**  
1. Display a navigation menu accessible from all screens.  
2. Include links to Profile, Habits, Reports, and Sign Out.  
3. Ensure smooth navigation without excessive page reloads.  

**Priority:** High  
**Story Points:** 2  
**Notes:**  
- The menu should be responsive and easy to use on both desktop and mobile devices.  

---

### User Story 8: Navigate to Profile
**Title:**  
_As a user, I want to navigate to my profile page from the menu so that I can view and update my personal information._  

**Acceptance Criteria:**  
1. Provide a menu option labeled "Profile" that directs users to their profile page.  
2. Ensure smooth navigation without excessive page reloads.  
3. Highlight the active menu option when the profile page is selected.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- The profile menu option should be easily accessible from all screens.  

---

### User Story 9: Navigate to Habits Page
**Title:**  
_As a user, I want to navigate to the habits page from the menu so that I can manage and track my daily habits._  

**Acceptance Criteria:**  
1. Provide a menu option labeled "Habits" that directs users to the habits page.  
2. Ensure smooth navigation without excessive page reloads.  
3. Highlight the active menu option when the habits page is selected.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- The habits menu option should be easily accessible from all screens.

---

### User Story 10: Sign Out from Menu
**Title:**  
_As a user, I want to sign out of my account using an option in the menu so that I can securely log out when I'm finished using the app._  

**Acceptance Criteria:**  
1. Display a Sign Out option in the menu.  
2. Ensure the user is redirected to the login screen upon signing out.  
3. Clear session data after logout.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- Users should receive a confirmation prompt before signing out to prevent accidental logouts.   

---

## Profile Page

### User Story 11: View Personal Information
**Title:**  
_As a user, I want to view my personal information on my profile page so that I can verify my details._  

**Acceptance Criteria:**  
1. Display user details such as name, email, and registration date.  
2. Ensure information is retrieved securely from the database.  
3. Allow users to access the profile page from the menu.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- Profile information should be displayed in a structured and readable format.  

---

### User Story 12: Edit Personal Information
**Title:**  
_As a user, I want to edit my personal information on my profile page so that I can keep my details up to date._  

**Acceptance Criteria:**  
1. Provide an edit option for fields such as name, email, and password.  
2. Ensure changes are validated before saving.  
3. Display a confirmation message upon successful update.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- Users should receive an error message if they enter invalid details.

---

### User Story 13: Save Updated Information
**Title:**  
_As a user, I want my updated personal information to be saved so that my changes are reflected across the app._  

**Acceptance Criteria:**  
1. Ensure that updated profile details persist after page reload or logout.  
2. Save changes securely in the database.  
3. Display a success message once the update is complete.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- Users should have the option to revert changes before saving.  

---

### User Story 14: Update Name in Header
**Title:**  
_As a user, I want my updated name to be displayed in the app's header so that my changes are immediately visible._  

**Acceptance Criteria:**  
1. Reflect name changes instantly in the app’s header after saving.  
2. Ensure name updates persist after logging out and logging back in.  
3. Update all instances where the user's name is displayed.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- Changes should be dynamically updated without requiring a page refresh.  

---

## Habits Page

### User Story 15: Add a New Habit
**Title:**  
_As a user, I want to add new habits on the details configuration page so that I can manage and update my habits as needed._  

**Acceptance Criteria:**  
1. Provide a form to add habit details.  
2. Save the habit and display it in the list.  
3. Allow editing of newly added habits.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- The system should provide predefined habit suggestions to help users get started.  

---

### User Story 16: Delete a Habit
**Title:**  
_As a user, I want to delete existing habits so that I can keep my habits up to date._  

**Acceptance Criteria:**  
1. Provide an option to delete a habit.  
2. Display a confirmation prompt before deletion.  
3. Ensure the habit is removed from the list.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- Deleted habits should be recoverable within a short time window to prevent accidental loss.  

---

### User Story 17: Personalize Habit with Color
**Title:**  
_As a user, I want to assign a specific color to each habit to make it personal to me._  

**Acceptance Criteria:**  
1. Provide a color selection option for habits.  
2. Apply the selected color to the habit display.  
3. Ensure the selected color persists across sessions.  

**Priority:** Low  
**Story Points:** 2  
**Notes:**  
- Users should have the option to reset the color to a default setting if needed.   

---

## Reports Page

### User Story 18: View Weekly Reports
**Title:**  
_As a user, I want to see a report of my weekly habit progress so that I can understand how well I am maintaining my habits._  

**Acceptance Criteria:**  
1. Display a summary of completed habits for the week.  
2. Provide graphical representations (e.g., bar charts, line graphs).  
3. Allow filtering by date range.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- The report should be easy to read and provide actionable insights.  

---

### User Story 19: View All Habits
**Title:**  
_As a user, I want to see both completed and incomplete habits in my report so that I have a comprehensive view of my habit tracking performance._  

**Acceptance Criteria:**  
1. List all habits with their completion status.  
2. Allow sorting and filtering options.  
3. Display habit trends over time.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- Users should be able to toggle between completed and incomplete habits for clarity.  

---

### User Story 20: Visualize Completed Habits
**Title:**  
_As a user, I want to see a chart of my completed habits for each day of the week so that I can quickly identify trends in my progress._  

**Acceptance Criteria:**  
1. Display a chart showing daily habit completion.  
2. Provide an option to view different timeframes (weekly, monthly).  
3. Ensure the chart updates dynamically as new data is recorded.  

**Priority:** High  
**Story Points:** 3  
**Notes:**  
- The chart should be visually appealing and support different display formats (bar, line, pie chart).  

---

## Notifications Page

### User Story 21: Enable/Disable Notifications
**Title:**  
_As a user, I want to be able to enable or disable notifications for the app so that I can control my reminder preferences._  

**Acceptance Criteria:**  
1. Provide a toggle switch to enable or disable notifications.  
2. Ensure settings persist after app restarts.  
3. Display a confirmation message upon saving changes.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- Notifications should be configurable to avoid unnecessary alerts.  

---

### User Story 22: Add Habits for Notifications
**Title:**  
_As a user, I want to select specific habits to receive notifications for so that I only get reminders for the habits I am actively working on._  

**Acceptance Criteria:**  
1. Provide an option to enable notifications for individual habits.  
2. Ensure users can toggle notifications on or off for each habit.  
3. Display a confirmation message after saving notification preferences.  

**Priority:** Medium  
**Story Points:** 2  
**Notes:**  
- Users should be able to change notification preferences at any time.  

---

### User Story 23: Set Notification Times
**Title:**  
_As a user, I want to set specific times for habit notifications so that I receive reminders at the most convenient moments._  

**Acceptance Criteria:**  
1. Allow users to select custom notification times for each habit.  
2. Provide default options (morning, afternoon, evening) for convenience.  
3. Ensure notifications are delivered at the scheduled times.  

**Priority:** Medium  
**Story Points:** 3  
**Notes:**  
- Users should be able to edit or remove scheduled notifications at any time.

---
