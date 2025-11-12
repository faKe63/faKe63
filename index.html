<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <title>Feliz Aniversário!</title>
    <style>
        *, *::before, *::after { box-sizing: border-box; }

        :root {
            --bg-color:       #7a3631;
            --text-color:     #f5f5f5;
            --accent-color:   #ffa500;
            --success-bg:     #4caf50;
            --error-color:    #ff6b6b;
            --success-color:  #ff6347;
        }

        body {
            margin: 0;
            font-family: system-ui, sans-serif;
            text-align: center;
            padding: 5vh 1rem;
            background: var(--bg-color);
            color: var(--text-color);
        }

        h1 { margin-bottom: 1rem; }

        label { display: inline-block; margin-bottom: .5rem; font-weight: 600; }

        #age-input {
            padding: .5rem;
            font-size: 1rem;
            width: 120px;
            text-align: center;
            border: 2px solid #ccc;
            border-radius: 4px;
        }

        #submit-button {
            padding: .75rem 1.5rem;
            font-size: 1rem;
            cursor: pointer;
            background: var(--accent-color);
            color: #fff;
            border: none;
            border-radius: .5rem;
            margin-left: .5rem;
            transition: background .3s ease;
        }
        #submit-button:disabled,
        #submit-button[aria-disabled="true"] {
            background: var(--success-bg);
            cursor: default;
        }

        .error {
            color: var(--error-color);
            margin-top: .5rem;
        }
        .success {
            font-size: 2rem;
            color: var(--success-color);
            font-weight: bold;
            margin-top: 1rem;
        }

        /* Footer */
        #page-footer {
            margin-top: 3rem;
            padding: 1rem 0;
            background: rgba(0,0,0,.15);
            color: var(--text-color);
            font-size: .9rem;
        }
        #page-footer a {
            color: #ffd966;
            text-decoration: underline;
        }
        #page-footer a:hover { color: #ffea00; }

        @media (max-width:480px){
            body{padding-top:2rem;}
            #age-input{width:80%;}
        }
    </style>
</head>
<body>
    <h1>Atenção!!<br>O Recipiente desta Mensagem (não) é normal.</h1>

    <label for="age-input">Desbloqueia esta Mensagem:</label>
    <input type="number" id="age-input" min="0" max="110" placeholder="Idade" required>
    <button id="submit-button">Sou Velho</button>

    <div id="error-message" class="error" role="alert" aria-live="assertive"></div>
    <div id="message-area"></div>

    <footer id="page-footer">
        Made <a href="https://www.instagram.com/rafasoares115/" target="_blank" rel="noopener">byfaKe</a> with
        ❤️
    </footer>

    <script>
        const CORRECT_AGE = 36;
        const GIF_HTML = `
            <img src="https://media.giphy.com/media/v1.Y2lkPWVjZjA1ZTQ3eDc3Zm94MGt6Nm1uMHY3Z3cyd2VkaXRhanI1ODJ6YjB6bmt2YW8xbyZlcD12MV9naWZzX3NlYXJjaCZjdD1n/ioWaevqsBvyD8O4VAW/giphy.gif"
                 alt="Animação de aniversário"
                 style="width:250px;margin-top:20px;">
        `;
        const FINAL_MESSAGE = `
            🎉🎉 Muitos parabéns (ainda sabes a tua idade!)<br>
            Um Feliz Aniversário Gaiato Panuco 😘😘 🎉🎉<br><br>
            ${GIF_HTML}
        `;

        const ageInput    = document.getElementById('age-input');
        const submitBtn   = document.getElementById('submit-button');
        const errorDiv    = document.getElementById('error-message');
        const messageArea = document.getElementById('message-area');

        function clearError(){ errorDiv.textContent=''; errorDiv.removeAttribute('role'); }
        function setError(msg){ errorDiv.textContent=msg; errorDiv.setAttribute('role','alert'); }

        submitBtn.addEventListener('click',()=>{
            const raw = ageInput.value.trim(); clearError();
            if(raw===''){ setError('Isso está grave, nem sabes a tua idade!'); return; }
            const age = Number(raw);
            if(Number.isNaN(age) || !Number.isInteger(age)){
                setError('Isso está grave, nem sabes a tua idade!');
                return;
            }
            if(age===CORRECT_AGE){
                submitBtn.disabled=true;
                submitBtn.setAttribute('aria-disabled','true');
                submitBtn.textContent="😘😘😘😘😘";
                messageArea.innerHTML=`<p class="success">${FINAL_MESSAGE}</p>`;
            }else{
                setError('Isso está grave, nem sabes a tua idade!');
            }
        });
    </script>
</body>
</html>
