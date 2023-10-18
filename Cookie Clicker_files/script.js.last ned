const countElement = document.getElementById('count');
const plusOne = document.getElementById('plusOne');
const minusOne = document.getElementById('minusOne');

let count = 0;
const zerothMessage = document.createElement("p")
const actualActualFirstMessage = document.createElement("p")
const actualFirstMessage = document.createElement("p")
const firstMessage = document.createElement("p");
const secondMessage = document.createElement("p");
const secondAndAHalfMessage = document.createElement("p")
const thirdMessage = document.createElement("p");

function increaseCount() {
    if (count >= 3000) {
        count += 100;
        thirdMessage.textContent = "Congratulations on reaching 3000 clicks! You did it!"
        thirdMessage.classList.add("thirdMessageStyling");
        document.body.appendChild(thirdMessage);
    } else if (count >= 1500) {
        count += 75;
        secondAndAHalfMessage.textContent = "Congratulations on reaching 1500 clicks! Keep clicking just a bit more!"
        secondAndAHalfMessage.classList.add("secondAndAHalfMessageStyling");
        document.body.appendChild(secondAndAHalfMessage);
    } else if (count >= 500) {
        count += 50;
        secondMessage.textContent = "Congratulations on reaching 500 clicks! Keep clicking!"
        secondMessage.classList.add("secondMessageStyling");
        document.body.appendChild(secondMessage);
    } else if (count >= 100) {
        count += 10;
        firstMessage.textContent = "Congratulations on reaching 100 clicks! Keep clicking!"
        firstMessage.classList.add("firstMessageStyling");
        document.body.appendChild(firstMessage);
    } else if (count >= 50) {
        count += 2
        actualFirstMessage.textContent = "Congratulations on reaching 50 clicks! Keep clicking!"
        actualFirstMessage.classList.add("actualFirstMessageStyling");
        document.body.appendChild(actualFirstMessage);
    } else if (count >=25) {
        count += 1
        actualActualFirstMessage.textContent = "Congratulations on reaching 25 clicks! Keep clicking!"
        document.body.appendChild(actualActualFirstMessage);
    } else if (count >=5) {
        count += 1
        zerothMessage.textContent = "Congratulations on reaching 5 clicks! Keep clicking!"
        document.body.appendChild(zerothMessage);
    } else { 
        count++;
    }
    countElement.textContent = count;
}
   
function decreaseCount() {
    count--;
    countElement.textContent = count;
}

plusOne.addEventListener('click', increaseCount);
minusOne.addEventListener('click', decreaseCount);