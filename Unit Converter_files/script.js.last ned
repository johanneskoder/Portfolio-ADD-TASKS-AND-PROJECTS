// Unit Converter

// First: Declare our global-scope variables

const fromUnit = document.getElementById("from");
const toUnit = document.getElementById("to");
const button = document.getElementById("convertBtn");
const input = document.getElementById("userInput");

function convert() {
    const inputValue = parseInt(input.value);
    const fromUnitValue = fromUnit.value;
    const toUnitValue = toUnit.value;
    let result = ""

    if (fromUnitValue === "meters"
    && toUnitValue === "kilometers") {
        result = inputValue / 1000
    } else if (fromUnitValue === "meters" && toUnitValue === "miles") {
        result = inputValue * 0.000621371;
    } else if (fromUnitValue === "kilometers" && toUnitValue === "meters") {
        result = inputValue * 1000;
    } else if (fromUnitValue === "kilometers" && toUnitValue === "miles") {
        result = inputValue * 0.621371;
    } else if (fromUnitValue === "miles" && toUnitValue === "meters") {
        result = inputValue * 1609.34;
    } else if (fromUnitValue === "miles" && toUnitValue === "kilometers") {
        result = inputValue * 1.609344;
    }

    document.getElementById("output").textContent = result.toFixed(2);
}

fromUnit.addEventListener("change", sameUnits)
toUnit.addEventListener("change", sameUnits)

function sameUnits() {
    if (fromUnit.value === toUnit.value) {
        button.disabled = true;
    } else {
        button.disabled = false;
    }
}

button.addEventListener("click", convert)



