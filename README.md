# CALCULATOR-JS
Calculator javascript
function backscape() {
    const display = document.getElementById("display");
    if (display) {
        display.value = display.value.slice(0, -1);
    }
}

function calculatPercentage() {
    const display = document.getElementById("display");
    if (display) {
        const number = parseFloat (display.value);
        const lastCharacter = display.value.slice(-1);
        if (lastCharacter === '%') {
            const result = (numberWithPercentage / 100) * number;
            display.value = result;
        } else {
            const result = number / 100;
            display.value = result + '%';
        }
    }
}

function addToDisplay(value) {
    const display = document.getElementById("display");
    if (display) {
        display.value += value;
    }
}

function clearDisplay() {
    const display = document.getElementById("display");
    if (display) {
        display.value = '';
    }
}
