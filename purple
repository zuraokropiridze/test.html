!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <title>purple</title>
    <link rel="stylesheet" href="test.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>

    <input type="checkbox" id="page-switcher">
    <input type="checkbox" id="form-toggler">

    <div class="auth-wrapper">
        <div class="card">
            <div class="login-box">
                <h2>შესვლა</h2>
                <input type="email" placeholder="ელ-ფოსტა">
                <input type="password" placeholder="პაროლი">
                <label for="page-switcher" class="purple-btn">ავტორიზაცია</label>
                <p>არ გაქვს ანგარიში? <label for="form-toggler" class="toggle-link">დარეგისტრირდი</label></p>
            </div>

            <div class="signup-box">
                <h2>რეგისტრაცია</h2>
                <input type="text" placeholder="სახელი">
                <input type="text" placeholder="გვარი">
                <input type="email" placeholder="ელ-ფოსტა">
                <input type="tel" placeholder="ტელეფონის ნომერი">
                <input type="password" placeholder="პაროლი">
                <label for="page-switcher" class="purple-btn">შექმენი ანგარიში</label>
                <p>უკვე გაქვს ანგარიში? <label for="form-toggler" class="toggle-link">შესვლა</label></p>
            </div>
        </div>
    </div>

    <div class="app-screen">
        <nav class="side-nav">
            <div class="nav-icon active" title="მთავარი"><i class="fas fa-home"></i></div>
            <div class="nav-icon" title="Reels"><i class="fas fa-play-circle"></i></div>
            <div class="nav-icon" title="მესიჯები"><i class="fas fa-paper-plane"></i></div> 
            <div class="nav-icon" title="პროფილი"><i class="fas fa-user-circle"></i></div>
            <label for="page-switcher" class="nav-icon logout"><i class="fas fa-sign-out-alt"></i></label>
        </nav>

        <main class="main-content">
            <header>
                <h1>მოგესალმებით!</h1>
                <p style="color: #888;">თქვენი შეტყობინებები და სიახლეები ერთ სივრცეში.</p>
            </header>
            <div class="reels-row">
                <div class="reel-demo">Reel 1</div>
                <div class="reel-demo">Reel 2</div>
                <div class="reel-demo">Reel 3</div>
            </div>
        </main>
    </div>

</body>
</html>



:root {
    --bg-main: #121212;
    --bg-card: #1e1e1e;
    --purple: #7b2cbf;
    --purple-hover: #9d4edd;
    --text: #ffffff;
}

body, html {
    margin: 0; padding: 0;
    height: 100%;
    background: var(--bg-main);
    color: var(--text);
    font-family: 'Segoe UI', sans-serif;
    overflow: hidden;
}

#page-switcher, #form-toggler { display: none; }


.signup-box { display: none; }
#form-toggler:checked ~ .auth-wrapper .login-box { display: none; }
#form-toggler:checked ~ .auth-wrapper .signup-box { display: block; }

.auth-wrapper {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.card {
    background: var(--bg-card);
    padding: 35px;
    border-radius: 20px;
    width: 350px;
    text-align: center;
    border: 1px solid #333;
}

input {
    width: 100%;
    padding: 12px;
    margin: 8px 0;
    background: #252525;
    border: 1px solid transparent;
    border-radius: 10px;
    color: white;
    box-sizing: border-box;
}

.purple-btn {
    display: block;
    background: var(--purple);
    padding: 12px;
    margin-top: 15px;
    border-radius: 10px;
    cursor: pointer;
    font-weight: bold;
    transition: 0.2s;
}

.purple-btn:active { transform: scale(0.94); } 

.toggle-link { color: var(--purple-hover); cursor: pointer; text-decoration: underline; }


.app-screen {
    position: fixed;
    top: 0; left: 0; width: 100%; height: 100%;
    background: var(--bg-main);
    display: flex;
    transform: translateY(100%);
    transition: 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}

#page-switcher:checked ~ .app-screen { transform: translateY(0); }

.side-nav {
    width: 80px;
    background: var(--bg-card);
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 20px;
    border-right: 1px solid #333;
}

.nav-icon {
    font-size: 24px;
    color: #555;
    margin: 20px 0;
    cursor: pointer;
    transition: 0.3s ease;
}


.nav-icon:hover {
    color: var(--purple-hover);
    transform: scale(1.2);
}

.nav-icon:active {
    color: white;
    transform: scale(0.8);
}

.nav-icon.active { color: var(--purple); }

.main-content { padding: 40px; flex: 1; }
.reels-row { display: flex; gap: 15px; margin-top: 20px; }
.reel-demo {
    width: 150px; height: 250px;
    background: #252525;
    border-radius: 15px;
    border: 1px solid #333;
    transition: 0.3s;
}
.reel-demo:hover { border-color: var(--purple); }
.logout { margin-top: auto; padding-bottom: 20px; color: #cc3333; }
