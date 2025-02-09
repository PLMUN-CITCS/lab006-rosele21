# 2025-ITELEC2-LAB006
Week 02 - Python Variables, Operators and I/O Statements

Laboratory # 06 - Utilizing Basic Math Libraries in Python

## **Instructions**

### **Step 1.1: Accept the Assignment**

   1. Click on the assignment link provided by your instructor.
   2. GitHub Classroom will create a **private repository** under your GitHub account.
   3. After the repository is created, click **"Go to Repository"** to view your assignment.

---

### **Step 1.2: Setup your Git Environment**
Only perform this if this is the first time you will setup your Git Environment

   1. Create a GitHub Account:
   ```bash
   https://github.com/signup?source=login
   ```
      
   2. Download and Install Git on your Laptop/Desktop:
   ```bash
   https://git-scm.com/downloads
   ```
   
   3. Create a Folder in your Laptop/Desktop
   4. Right-click anywhere in the created folder and select "Open Git Bash Here".
   5. In the Git Bash Terminal, set your git name, perform command:
   ```bash
   git config --global user.name "Your Name"
   ```
   
   6. In the Git Bash Terminal, set your git email, perform command:
   ```bash
   git config --global user.email "your.email@example.com"
   ```
   
   7. Create your SSH Key, just follow the instructions, no need to provide filename and passphrase. In the Git Bash Terminal, perform command:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
   
   8. Copy your SSH Keys into clipboard. In the Git Bash Terminal, perform command:
   ```bash
   clip < ~/.ssh/id_rsa.pub
   ```
   
   9. Log in to your GitHub account.
   10. In the upper-right corner of GitHub, click your profile picture and select Settings.
   11. In the left sidebar, click on SSH and GPG keys.
   12. Click the New SSH key button.
   13. In the Title field, give the key a recognizable name (e.g., "My Windows Laptop").
   14. In the Key field, CTRL + V or paste the keys copied into your clipboard. Save the key.
   15. Go Back to terminal, use command:
   ```bash
   ssh -T git@github.com
   ```

### **Step 2: Clone the Repository to Your Local Machine**

   1. On your repository page, click the green **"Code"** button.
   2. Copy the repository URL (choose HTTPS for simplicity).
   3. Open your terminal (or Git Bash, Command Prompt, or PowerShell) and run:
   
   ```bash
   git clone <git_repo_url>
   ```
   
   4. Navigate into the cloned folder:
   
   ```bash
   cd <git_cloned_folder>
   ```

### **Step 3: Complete the Assignment**

**Laboratory # 06 - Utilizing Basic Math Libraries in Python**

   **Objective:**
   This exercise aims to introduce you to Python's math module and demonstrate how to use it to perform common mathematical operations, including: 
   - Calculating the square root of a number.
   - Obtaining the value of pi (π).
   - Converting degrees to radians.
   - Calculating the sine of an angle.

   **Desired Output:**
   ```bash
   Square root of 16 is: 4.0
   Value of pi is: 3.141592653589793
   Sine of 30 degrees (in radians) is: 0.49999999999999994
   Cosine of 60 degrees (in radians) is: 0.8660254037844387
   Tangent of 45 degrees (in radians) is: 0.5773502691896257
   Exponential of 2 is: 7.38905609893065
   Logarithm (base e) of 10 is: 2.302585092994046
   Logarithm (base 10) of 100 is: 2.0
   ```
      
   **Notable Observations (to be discussed after completing the exercise):**
   - The math module provides a wide range of mathematical functions.
   - You must import the math module before you can use its functions.
   - The math.sqrt() function calculates the square root of a number.
   - math.pi is a constant that stores the value of π.
   - Trigonometric functions (like math.sin(), math.cos(), math.tan()) expect arguments in radians, not degrees. Use math.radians() to convert from degrees to radians.
   - math.exp() calculates the exponential of a number (e raised to that number).
   - math.log() calculates the natural logarithm (base e) by default. You can provide a second argument to specify a different base (e.g., base 10).

   **Python Best Practices**
   - Import What You Need: Use import math to access math functions. Don't import everything if you only need a few things (though it's fine in this case).
   - Radians Matter: Trigonometric functions (sin, cos, tan) use radians, not degrees. Use math.radians() to convert.
   - Constants are Useful: math.pi gives you the value of pi. Use it directly instead of typing it out (mistakes are easy!).
   - Functions are Tools: math.sqrt(), math.exp(), math.log() are pre-built tools. Use them! Don't reinvent the wheel.
   - Check Your Answers: Make sure your results match what you expect. This helps catch mistakes early.
   - Explore: The math module has lots more functions. Look at the documentation to discover them!
   
   **Step-by-Step Instructions:**

   1. Setting up: Open your preferred Python environment or Text Editor, and create a Python Script.
      - Required Filename: `exercise_04.py`
      
   2.  Import the math module:
      - Use the import statement to import the math module. This makes the functions and constants within the math module available to your code.
```python
import math
```
      
   3.  Calculate the square root:
      - Choose a number (e.g., 16) and store it in a variable.
      - Use the math.sqrt() function to calculate the square root of the number. Store the result in a variable.
```python
number = 16
sqrt_result = math.sqrt(number)
```

   4. Get the value of pi:
      - Access the math.pi constant to get the value of π. Store it in a variable.
```python
pi_value = math.pi
```

   5. Calculate the sine of an angle:
      - Use the math.radians() function to convert the angle from degrees to radians. Store the result in a variable.
      - Use the math.sin() function to calculate the sine of the angle (in radians). Store the result in a variable.
```python
angle_degrees = 30
angle_radians = math.radians(angle_degrees)
sin_result = math.sin(angle_radians)
```

   6. Calculate the cosine and tangent of an angle:
      - Use math.cos() and math.tan() to calculate the cosine and tangent of the same angle (in radians). Store the results in variables.
```python
cos_result = math.cos(angle_radians)
tan_result = math.tan(angle_radians)
```
         
   7. Calculate the exponential and logarithms:
      - Use math.exp() to calculate the exponential of a number (e.g., 2). Store the result in a variable.
      - Use math.log() to calculate the natural logarithm (base e) of a number (e.g., 10). Store the result in a variable.
      - Use math.log(x, base) to calculate the logarithm of x with a specified base (e.g., base 10 of 100). Store the result in a variable.
```python
exp_result = math.exp(2)
log_result = math.log(10)  # Natural log (base e)
log10_result = math.log(100, 10) # Log base 10
```
         
   8. Display the results:
      - Use the print() function to display the results of all the calculations with descriptive labels.
```python
print("Square root of", number, "is:", sqrt_result)
print("Value of pi is:", pi_value)
print("Sine of 30 degrees (in radians) is:", sin_result)
print("Cosine of 60 degrees (in radians) is:", cos_result)
print("Tangent of 45 degrees (in radians) is:", tan_result)
print("Exponential of 2 is:", exp_result)
print("Logarithm (base e) of 10 is:", log_result)
print("Logarithm (base 10) of 100 is:", log10_result)
```

   9. Run the code: Execute your Python code.
   10. Observe the output: Compare your output with the "Desired Output" shown above.
   11. Discussion (Notable Observations): Discuss all the points in the "Notable Observations" section.  Why is it important to convert degrees to radians before using trigonometric functions?  What other functions are available in the math module?  (Encourage students to explore the documentation.)

### **Step 4: Push Changes to GitHub**
Once you've completed your changes, follow these steps to upload your work to your GitHub repository.

1. Check the status of your changes:
   Open the terminal and run:
   
```bash
git status
```
   This command shows any modified or new files.
   
2. Stage the changes:
   Add all modified files to staging:
   
```bash
git add .
```
   
3. Commit your changes:
   Write a meaningful commit message:
   
```bash
git commit -m "Submitting Python Week 02 - Session 01 - Exercise 04"
```
   
4. Push your changes to GitHub:
   Upload your changes to your remote repository:
   
```bash
git push origin main
```
