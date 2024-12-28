### README: Health Connect Android Application

---

#### **Project Name:** Health Connect  

#### **Description:**
Health Connect is an Android application designed to manage and track medical records, appointments, consultations, medication logs, and patient details. It offers a user-friendly interface, well-structured navigation, and functionality for medical tracking and data management.

---

### **Project Structure**

#### **Directories & Files:**
1. **`manifests/AndroidManifest.xml`**
   - Defines all application activities and configurations.
   - Entry point: `splashScreen` activity navigates to the `MainActivity`.

2. **`java/com.example.myapplication`**
   - **`MainActivity`**: The main entry point post-splash screen. Displays the home page with navigation buttons.
   - **`splashScreen`**: Handles the splash screen animation and transitions to `MainActivity`.
   - **`testing`**: A utility activity for testing the project setup.

3. **`res/layout/`**
   - **`activity_main.xml`**: Layout for the main home page displaying navigational buttons.
   - **`splashscreen.xml`**: Layout for the splash screen with animated components.
   - **Patient Management Layouts:**
     - `add_patient.xml`, `patient_item.xml`, `patient_details.xml`
   - **Appointment Management Layouts:**
     - `add_appointment.xml`, `appointment_list.xml`, `appointment_item.xml`
   - **Medication Management Layouts:**
     - `add_medication.xml`, `medicine_list_item.xml`, `medication_log_item.xml`, `medication_history.xml`
   - **Consultation Management Layouts:**
     - `add_consultation.xml`, `consultation_item.xml`, `consult_history.xml`

4. **`res/anim/`**
   - **`fade_in.xml`**: Animation for fading in UI elements.
   - **`slide_up.xml`**: Animation for sliding UI elements upward.

5. **`res/mipmap/`**
   - Contains app icons for various resolutions.

6. **`res/drawable/`**
   - Holds images and icons used throughout the application.

---

### **Setup Instructions**

1. **Prerequisites:**
   - Android Studio installed.
   - Android SDK configured (minimum API level 23, target API 34).

2. **Cloning the Repository:**
   ```bash
   git clone https://github.com/Epi-Nabeel/HealthConnect
   cd HealthConnect
   ```

3. **Configuring SDK:**
   - Open `local.properties` file in the project root.
   - Add the following:
     ```
     sdk.dir=<path-to-android-sdk>
     ```

4. **Running the App:**
   - Open the project in Android Studio.
   - Sync Gradle files.
   - Run the project on an emulator or connected device.

---

### **Features**

1. **Splash Screen:**
   - Animated splash screen with fade-in and slide-up effects.
   - Auto-transitions to the main activity after 3 seconds.

2. **Home Page:**
   - **Buttons for navigation**:
     - **Patient Records**: Navigate to manage patient records.
     - **Consultations**: Navigate to consultation logs.
     - **Medical Tracking**: Access medication logs.
     - **Appointments**: View and manage appointments.
     - **Reports**: Access medical reports.

3. **Modular Layouts:**
   - Each module has its dedicated layout files for adding, viewing, and editing records.

4. **Animations:**
   - Smooth fade-in and slide-up animations enhance user experience.

---

### **How Navigation Works**

1. **Splash to Home:**
   - **Code:** `splashScreen.java`
   - **Details:** Splash screen transitions to the `MainActivity` with animations.

2. **Home Page Navigation:**
   - Buttons implemented using `CardView` trigger intents to navigate to respective activities:
     - Example: `Patient Records` button navigates to the patient management activity.

3. **Testing Activity:**
   - A utility activity for testing components independently.

---

### **Dependencies**

1. **AppCompat Library:**
   - Used for backward compatibility of UI components.

2. **ConstraintLayout:**
   - For designing flexible and adaptive layouts.

3. **CardView:**
   - For creating navigational buttons with shadow effects.

4. **AnimationUtils:**
   - For implementing smooth transitions and animations.

---


### **Screenshots**

1. **Homepage:**  
   ![Homepage](https://github.com/Epi-Nabeel/HealthConnect/blob/main/screenshots/Screenshot%202024-12-28%20094936.png)

2. **Patient Records:**  
   ![Patient Records](https://github.com/Epi-Nabeel/HealthConnect/blob/main/screenshots/Screenshot%202024-12-28%20100251.png)

3. **Consultation History:**  
   ![Consultation](https://github.com/Epi-Nabeel/HealthConnect/blob/main/screenshots/Screenshot%202024-12-28%20100304.png)

4. **Medical Tracking:**  
   ![Medical Tracking](https://github.com/Epi-Nabeel/HealthConnect/blob/main/screenshots/Screenshot%202024-12-28%20100315.png)

5. **Appointments:**  
   ![Appointments](https://github.com/Epi-Nabeel/HealthConnect/blob/main/screenshots/Screenshot%202024-12-28%20100324.png)

6. **Medicine List:**  
   ![Medicine List](https://github.com/Epi-Nabeel/HealthConnect/blob/main/screenshots/Screenshot%202024-12-28%20100335.png)

---


### **Contributions**

Contributors can follow these steps to contribute:
1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Commit changes with proper commit messages.
4. Create a pull request for review.

---

### **License**
This project is licensed under the MIT License. You are free to use and modify the code with proper attribution.

---

### **Acknowledgments**
- **Android Documentation** for detailed guidance on activities, layouts, and animations.
- Stack Overflow for debugging assistance.

---

Feel free to customize or expand the README further! Let me know if you need any additional sections or details. 😊
