<!DOCTYPE html>
<html>
<head>
    <title>MensagemSecreta byfaKe</title>
    <style>
        body { font-family: sans-serif; text-align: center; padding-top: 50px; background-color: #7a3631; }
        #message-area { margin-top: 30px; font-size: 24px; color: #333; }
        #age-input { padding: 8px; font-size: 16px; width: 100px; text-align: center; }
        #submit-button { padding: 10px 20px; font-size: 18px; cursor: pointer; background-color: #FFA500; color: white; border: none; border-radius: 5px; margin-left: 10px; }
        .error { color: red; margin-top: 10px; }
        .success { font-size: 36px; color: #ff6347; font-weight: bold; }
    </style>
</head>
<body>

    <h1>Atenção!!<br>O Recipiente desta Mensagem (não) é normal.</h1>
    
    <label for="age-input">Desbloqueia esta Mensagem:</label>
    <input type="number" id="age-input" min="0" max="110" value="" placeholder="Idade">
    <button id="submit-button">Sou Velho</button>
    
    <div id="error-message" class="error"></div>
    <div id="message-area"></div>

    <script>
        const correctAge = 36;

        const gifHtml = '<img src="https://media.giphy.com/media/v1.Y2lkPWVjZjA1ZTQ3eDc3Zm94MGt6Nm1uMHY3Z3cyd2VkaXRhanI1ODJ6YjB6bmt2YW8xbyZlcD12MV9naWZzX3NlYXJjaCZjdD1n/ioWaevqsBvyD8O4VAW/giphy.gif" alt="A GIF" style="width: 250px; margin-top: 20px;">';

        const finalMessage = "🎉🎉 Muitos parabéns (ainda sabes a tua idade!) Um Feliz Aniversário Gaiato Panuco 😘😘 🎉🎉" + '<br><br>' + gifHtml;

        const ageInput = document.getElementById('age-input');
        const submitButton = document.getElementById('submit-button');
        const messageArea = document.getElementById('message-area');
        const errorMessage = document.getElementById('error-message');

        submitButton.onclick = function() {
            const inputAge = parseInt(ageInput.value);
            errorMessage.textContent = ''; // Clear previous errors

            if (inputAge === correctAge) {
                // Show the message
                submitButton.disabled = true;
                submitButton.textContent = "😘😘😘😘😘";
                submitButton.style.backgroundColor = '#4CAF50';
                messageArea.innerHTML = `<p class="success">${finalMessage}</p>`;
            } else if (isNaN(inputAge) || ageInput.value.trim() === '') {
                // Error: Empty
                errorMessage.textContent = 'Isso está grave, nem sabes a tua idade!';
            } else {
                // Error: Wrong
                errorMessage.textContent = 'Isso está grave, nem sabes a tua idade!';
            }
        };
    </script>

</body>
</html>
