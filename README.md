<!DOCTYPE html>
<html>
<head>
<title>System Scan</title>
<style>
body {
    background: black;
    color: #00ff00;
    font-family: "Courier New", monospace;
    padding: 20px;
    line-height: 1.5;
}
#terminal {
    white-space: pre-wrap;
    font-size: 16px;
}
.blink {
    animation: blink 0.8s infinite;
}
@keyframes blink {
    0% { opacity: 1; }
    50% { opacity: 0; }
    100% { opacity: 1; }
}
</style>
</head>
<body>

<div id="terminal">Initializing system...</div>

<script>
let lines = [
    "Connecting to device...",
    "Granting camera permissions...",
    "Accessing front camera module...",
    "Scanning face...",
    "Detecting identity...",
    "Cross-checking face in database...",
    "WARNING: Unusual activity detected!",
    "Tracing exact location...",
    "Capturing image...",
    "Processing...",
    "Uploading to server...",
    "ERROR: Unauthorized user detected!",
    "Preparing report...",
    "",
    "🤣 GOTCHA! THIS WAS A PRANK!!",
    "Tera camera to on hua bhi nahi 😆"
];

let index = 0;
function showLine() {
    if (index < lines.length) {
        document.getElementById("terminal").innerHTML += "\n" + lines[index];
        index++;
        setTimeout(showLine, 700);
    } else {
        document.getElementById("terminal").innerHTML += "\n\nPress back and rethink your life choices 😎";
    }
}

setTimeout(showLine, 1000);
</script>

</body>
</html>
