# Python-Donation-Clinic-Project

The **Blood Compatibility Checker** is a Python-powered tool designed to quickly determine blood type compatibility for donors and receivers.
With just a few inputs, users can discover who they can donate to or receive blood from,
making it perfect for educational purposes or as a handy reference for medical contexts.

---

## 🚀 Features
- **🔍 Donor Compatibility**: Find out which blood types you can donate to based on your blood type.
- **📥 Receiver Compatibility**: Learn which blood types you can receive from.
- **🤖 Interactive User Input**: A simple terminal-based interface to enter your details and get instant results.
- **⚠️ Error Handling**: Validates inputs to ensure a smooth and frustration-free experience.

---

## 📂 Project Structure
### 1. Compatibility Rules
Two dictionaries store compatibility data:
- `donor_compatibility`: Maps blood types to the types they can donate to.
- `receiver_compatibility`: Maps blood types to the types they can receive from.

### 2. Main Functionality
- **Input Collection**: Gathers the user's name, role (donor or receiver), and blood type.
- **Validation**: Checks for valid roles and blood types.
- **Compatibility Display**: Outputs personalized results based on the input.

### 3. Execution
- Fully interactive, running in a terminal or command-line environment.
- Provides real-time compatibility feedback.

---

## 📖 Try it yourself!
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Blood-Compatibility-Checker.git
   cd Blood-Compatibility-Checker
   ```
2. Run the program:
   ```bash
   python blood_compatibility.py
   ```
3. Follow the prompts:
   - Enter your name.
   - Specify if you’re a donor (`D`) or receiver (`R`).
   - Provide your blood type (e.g., `A+`, `O-`).
4. Get instant results on compatibility!

---

## 💻 Example Outputs

### Donor Compatibility
**Input**:
```
Enter your first name and last name: Matheus Alonso
Are you a donor or receiver? (D/R): D
Enter your blood type: B+
```

**Output**:
```
As a donor, you can give: B+ AB+
```

### Receiver Compatibility
**Input**:
```
Enter your first name and last name: Fulano detal
Are you a donor or receiver? (D/R): R
Enter your blood type: AB+
```

**Output**:
```
As a receiver, you can receive: A+ A- B+ B- AB+ AB- O+ O-
```

### Error Handling
**Input**:
```
Enter your blood type: XZ
```

**Output**:
```
Invalid blood type.
```

---

## 🌟 Why This Project?
I created this project to showcase my coding abilities using Python and as a part of my long term goal of having a high-quality Github Portfolio

---

## Challenges
Although simple, the part I struggled the most in this part was creating and understanding how libraries work. Using trial and error I was able to get a 
good grasp of its usage and usability cases.

## 🛠️ Future Enhancements
- Add a graphical user interface (GUI) for an enhanced user experience.
- Integrate a database for storing user profiles and donation records.
- Expand functionality to support Rh factor compatibility details.

---

## 🩸 Compatibility Rules
### Donor Compatibility:
| Blood Type | Can Donate To         |
|------------|-----------------------|
| A+         | A+, AB+              |
| A-         | A+, A-, AB+, AB-     |
| B+         | B+, AB+              |
| B-         | B+, B-, AB+, AB-     |
| AB+        | AB+                  |
| AB-        | AB+, AB-             |
| O+         | A+, B+, AB+, O+      |
| O-         | All blood types      |

### Receiver Compatibility:
| Blood Type | Can Receive From      |
|------------|-----------------------|
| A+         | A+, A-, O+, O-       |
| A-         | A-, O-               |
| B+         | B+, B-, O+, O-       |
| B-         | B-, O-               |
| AB+        | All blood types      |
| AB-        | A-, B-, AB-, O-      |
| O+         | O+, O-               |
| O-         | O-                   |
