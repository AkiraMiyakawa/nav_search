# Mapbox Navigation & Search Demo

This is a demonstration of Mapbox GL JS featuring map display, search, and routing (directions). 

Follow the steps below to get your own version running on the web.

---

## Step 1: Get Your Mapbox Access Token

1.  **Sign up:** Create a free account at [Mapbox.com](https://www.mapbox.com/).
2.  **Access Dashboard:** Go to your [Account Dashboard](https://account.mapbox.com/).
3.  **Copy Token:** Copy your **"Default public token"** (it should start with `pk.`).

---

## Step 2: Insert the Token into the Code

1.  Open the `index.html` file in your code editor or directly on GitHub.
2.  Locate **line 1940**. You will see the following line:
    ```javascript
    mapboxgl.accessToken = '<INPUT YOUR ACCESS TOKEN>';
    ```
3.  Replace `<INPUT YOUR ACCESS TOKEN>` with your actual token. It should look like this:
    ```javascript
    mapboxgl.accessToken = 'pk.eyJ1I...your_actual_token_here';
    ```
4.  **Commit and Push** the changes to your GitHub repository.

---

## Step 3: Deploy via GitHub Pages (Free Hosting)

1.  Go to your repository on GitHub.
2.  Click on the **"Settings"** tab (gear icon).
3.  In the left sidebar, click on **"Pages"**.
4.  Under **"Build and deployment" > "Branch"**, select the **`main`** branch (or `master`) and click **"Save"**.
5.  Wait for 1-2 minutes. Refresh the page until you see a message saying: 
    *“Your site is live at https://<your-username>.github.io/nav_search/”*
6.  Click that link to view your live map.

---

## ⚠️ Important: Security Warning

Since this is a client-side application, your Access Token will be visible in the browser's source code. To prevent others from using your token and consuming your free tier/quota, you **must** restrict your token:

1.  Go to your [Mapbox Access Tokens page](https://account.mapbox.com/access-tokens/).
2.  Edit your token.
3.  Under **"URL restrictions"**, add your GitHub Pages URL (e.g., `https://akiramiyakawa.github.io/`).
4.  Save the changes. This ensures the token only works on your specific domain.

---

## Original Project
Credit to [koheikanazawa](https://github.com/koheikanazawa/nav_search) for the original implementation.
