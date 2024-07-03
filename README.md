
# Real-Time Digital Clock
This project is a simple real-time digital clock that displays the current hours, minutes, and seconds. The time updates every second using JavaScript.

## Features
- Displays the current time in hours, minutes, and seconds.
- Updates the time every second.
- Pads single-digit hours, minutes, and seconds with a leading zero for a consistent two-digit display.

## How It Works
The JavaScript code uses the `setInterval` function to update the time every second. It retrieves the current time using the `Date` object and updates the HTML elements with the current hours, minutes, and seconds.

## Code Explanation
```javascript
let hrs = document.getElementById("hrs");
let min = document.getElementById("min");
let sec = document.getElementById("sec");

setInterval(() => {
    let currentTime = new Date();
    hrs.innerHTML = (currentTime.getHours() < 10 ? "0" : "") + currentTime.getHours();
    min.innerHTML = (currentTime.getMinutes() < 10 ? "0" : "") + currentTime.getMinutes();
    sec.innerHTML = (currentTime.getSeconds() < 10 ? "0" : "") + currentTime.getSeconds();
}, 1000)
```

###  Explanation
This section provides a detailed explanation of how the code works. The setInterval function is used to update the time every second. The Date object is used to get the current time, and the HTML elements are updated with the current hours, minutes, and seconds.

## Contributing
If you'd like to contribute to this project, please fork the repository and submit a pull request.

##  License
This project is licensed under the MIT License. See the LICENSE file for details.







