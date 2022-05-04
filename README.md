# Formul-rio-Faculdade
Formulário

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login_Tester</title>
    <link rel="stylesheet" href="./css/styles.css">
    <script src="./js/index.js" defer></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
    <script src="https://kit.fontawesome.com/8f1f1378d6.js" crossorigin="anonymous" defer></script>

</head>
<body>
    <header>
        <h1>Produção_Textual_Interdiciplinar</h1>
    </header>
    <main>
        <form>
            <section class="inputs-container">
                <input type="e-mail" placeholder="exemple@gmail.com">
                <div class="password-container">
                    <input type="password" id="field-password" class="field-password" placeholder="********">
                    <i class="fa-solid fa-eye" id="eye" onclick="showPassword()"></i>
                    <i class="fa-solid fa-eye-slash" id="eye-slash" onclick="showPassword()"></i>
                </div>
            </section>

            <section class="password-infos">
                <div>
                    <input type="checkbox">
                    <span>Lembrar senha?</span>
                </div>
                <a href="#">Esqueceu sua senha</a>
            </section>
            
            <button id="btn-login"> Login </button>
            <section class="links-container">
                <spam>Ou entre com:</spam>
                <aside>
                    <a href="#"><i class="fa-brands fa-google-plus-g google"></i></a>
                    <a href="#"><i class="fa-brands fa-facebook-square facebook"></i></a>
                    <a href="#"><i class="fa-brands fa-instagram instagram"></i></a>
                </aside>

            </section>
            
            <footer>
                <hr>
                <spam> Ainda não possui uma conta? <a href="#">Cadastre-se</a> </spam>
            </footer>
        </form>
    </main>
</body>
</html> 


Java Script

 function showPassoword() {
     const eye = document.getElementById('eye');
     const eyeSlash = document.getElementById('eye-slash');
     const fieldPassword = document.getElementById('field-password');

    if(eye.style.display === 'none') {
        eye.style.display = 'belock';
        yeSlash.style.display = 'none';
        fieldPassword.type - 'text';
    }else{
        eye.style.display = 'none';
        eyeSlash.style.display = 'block';
        fieldPassword.type - 'password';
    }
};


CSS

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins', sans-serif;
    text-decoration: none;
    color: #fff;
}

header{
    min-height: 9vh;
    display:flex;
    align-items: center;
    justify-content: center;
    background-color: #383c42;
}

header h1{
    font-size: 2.5em;
    color: #fff;
}
main{
    width: 100%;
    min-height: 100vh;
    background: linear-gradient(#18acfe, #0166e1);
    display: flex;
    justify-content: center;
    box-shadow: inset 0px 2px 3px rgba(0, 0, 0, 0.25);
}

main form{
    margin-top: 5%;
    width: 35%;
    height: 75vh;
    background-color: #383c42;
    box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.4) inset 0px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 18px;
    padding: 2%;
    
    display: flex;
    flex-direction: column;
    align-items: center;
}
main form .inputs-container{
    margin-top: 10%;
    width: 100%;

    display: flex;
    flex-direction: column;
    align-items: center;
}

main form .inputs-container input{
    width: 90%;
    height: 45px;
    padding: 8px 15px;
    border: 0;
    outline: 0;
    border-radius: 12px;
    
    font-size: 16px;
    color: #312e42;
    box-shadow: 00px 3px 3px rgba(0, 0, 0, 0.25);
}

main form .inputs-container input:focus{
    box-shadow: inset 1px 4px 7px rgba(0, 0, 0, 0.5);
}

main form .password-container{
    margin-top: 5%;
    width: 100%;
    position: relative;

    display: flex;
   flex-direction: column;
   align-items: center; 
}

main form .password-container i{
    position: absolute;
    right: 8%;
    top: 35%;
    color: #777;
    cursor: pointer;
}
 
main form .password-container #eye {
    display: none;
}

main form .password-infos{
    width: 90%;
    margin-top: 3%;

    display: flex;
    align-items: center;
    justify-content: space-between;
}

main form .password-infos a {
    transition: 0.2s ease-in-out;
}
main form .password-infos a:hover{
    color:#18acfe;
}

main form button{
    background-color: #18acfe;
    width: 90%;
    height: 10%;
    border: 0;
    outline: 0;
    border-radius: 12px;
    margin-top: 10%;
    font-size: 1.6em;
    font-weight: 600;
    cursor: pointer;
    transition: 0.3s ease-in-out;
}

main form button:hover{
    background: #fff;
    color: #18acfe;
}

main form .links-container{
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10%;
}

main form .links-container span{
    font-size: 0.8em;
    font-weight: 600;
}

main form .links-container aside{
    margin-top: 5%;
    width: 50%;
    display: flex;
    align-items: center;
    justify-content: space-around;
}

main form .links-container aside i{
    font-size: 1.6em;
    background-color: #fff;
    padding: 8px;
    height: 40px;
    width: 40px;
    border-radius: 20px;
    transition: 0.3 ease-in-out;
    color: #fff;

    display: flex;
    align-items: center;
    justify-content: center;
}

main form .links-container aside .google{
    color:#e34133;
}

main form .links-container aside .google:hover{
    color: #fff;
    background-color:#e34133;
}

main form .links-container aside .facebook{
    color:#14a0f9;
}

main form .links-container aside .facebook:hover{
    color: #fff;
    background-color:#14a0f9;
}

main form .links-container aside .instagram{
    color:#ff0095;
}

main form .links-container aside .instagram:hover{
    color: #fff;
    background-color:#ff0095;
}

main form footer{
    width: 100%;
    margin-top: 10%;

    display: flex;
    flex-direction: column;
    align-items: center;
}

main form footer hr{
    width: 100%;
    height: 3px;
    background-color: #fff;
}

main form footer span{
    font-weight: 400;
    font-size: 0.9em;
    margin-top: 5%;
}

main form footer a{
    font-weight: 600;
    transition: 0.2 ease-in-out;
}

main form footer a:hover{
    color:#18acfe;
}
