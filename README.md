Bunk Calculator 🎓

A sleek, modern web app to instantly calculate your class attendance percentage and determine exactly how many classes you can afford to "bunk" (or how many you need to attend to catch up!).

No more guessing—know your exact standing in seconds.

✨ Features

Current Attendance: Instantly see your current attendance percentage.

Smart Calculations:

Safe? 😎 Tells you exactly how many classes you can bunk in a row.

On the Edge? 😅 Warns you not to bunk any more classes.

In Danger? 😱 Calculates the precise number of classes you must attend to meet the requirement.

Visual Attendance Gauge: A color-coded progress bar (green, yellow, red) gives you a quick visual understanding of your attendance status.

Dynamic Icons: Get instant feedback with status emojis for success, warning, or danger.

Frosted Glass UI: A modern, fluid interface with subtle animations and a "frosted glass" effect.

Welcome Prompt: A fun, customizable welcome screen that can greet users or display special messages (like the "ADCET" one!).

🚀 Tech Stack

This project is built as a single, self-contained file with no dependencies, making it extremely lightweight and portable.

HTML5: For the core structure.

Tailwind CSS: For all styling, loaded via a CDN.

Vanilla JavaScript (ES6+): For all the logic, animations, and DOM manipulation.

🏃 How to Use

Open the bunk_calculator.html file in any modern web browser.

You'll see a welcome prompt. Enter your college acronym and proceed.

On the main calculator screen, fill in the three fields:

Required Attendance %: The minimum percentage your college requires (e.g., 75).

Total Lectures Held So Far: The total number of classes for that subject to date.

Lectures Attended So Far: The number of those classes you actually attended.

Click "Calculate".

Your result, including your percentage, the visual gauge, and your "bunk" or "attend" status, will appear instantly.

🔧 How to Modify

Changing the Special Welcome Message

Want to change the message for "ADCET" or add one for a different college? It's easy!

Open bunk_calculator.html.

Scroll to the bottom and find the <script> tag.

Look for the welcomeForm.addEventListener function (around line 200).

You can edit this block of code:

if (college === 'adcet') {
    // Show special message
    welcomeInputGroup.classList.add('hidden');

    // --- EDIT THIS LINE ---
    specialMessage.textContent = 'WOOOO!'; 
    // --- EDIT THIS LINE ---

    specialMessage.classList.remove('hidden');

    // Wait 1.5 seconds, then fade out
    setTimeout(startFadeOut, 1500);
} else {
    // ...
}


Change 'WOOOO!' to any message you want. You can also change the if (college === 'adcet') condition to target a different acronym.
