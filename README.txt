RRD WEBSITE: GO-LIVE GUIDE
==========================

WHAT'S IN THIS FOLDER
  index.html          The website (English + Arabic)
  content/site.json   All the text, photos, countries and contact details
  images/             Photos and the small browser-tab icon
  admin/              The editing screen  ->  www.rrdjo.com/admin
  netlify.toml        Hosting settings (leave as is)

You will create two free accounts: GitHub (stores the website files)
and Netlify (puts the website online). Allow about 45 minutes.

STEP 1  Put the files on GitHub
  1. Create a free account at github.com. Note your username.
  2. Click "+" (top right) > "New repository".
     Name: rrd-website   Visibility: Private   Click "Create repository".
  3. On the new page click "uploading an existing file".
     Drag in EVERYTHING inside this folder (index.html, content, images,
     admin, netlify.toml, README.txt), then click "Commit changes".
  4. Open admin/config.yml on GitHub, click the pencil icon, and change
        repo: YOUR-GITHUB-USERNAME/rrd-website
     to your username, e.g.  repo: rrd-jo/rrd-website
     Click "Commit changes".

STEP 2  Put the website online with Netlify
  1. Go to netlify.com > "Sign up" > "Sign up with GitHub".
  2. "Add new project" > "Import an existing project" > GitHub >
     choose rrd-website. Leave the build settings empty > "Deploy".
  3. After about a minute you get an address like rrd-website.netlify.app.
     Open it and check the site.

STEP 3  Turn on the editing screen login
  1. On GitHub: your photo (top right) > Settings > Developer settings >
     OAuth Apps > "New OAuth App".
       Application name:            RRD website editor
       Homepage URL:                https://www.rrdjo.com
       Authorization callback URL:  https://api.netlify.com/auth/done
     Click "Register application", then "Generate a new client secret".
     Keep this page open.
  2. On Netlify: your project > Project configuration > Access & security >
     OAuth > "Install a provider" > GitHub. Paste the Client ID and the
     Client secret from GitHub. Save.
  3. Open  https://rrd-website.netlify.app/admin  and click
     "Login with GitHub". You will see all sections of the site.

STEP 4  Receive quote requests by email
  1. Netlify > your project > Forms > "Enable form detection".
  2. Go to Deploys > "Trigger deploy" > "Deploy project" (once).
  3. Forms > Form notifications > "Add notification" > Email notification
     > enter info@rrdjo.com.
  Requests sent from the website now arrive in that inbox.

STEP 5  Use your own address www.rrdjo.com
  1. Netlify > Domain management > "Add a domain" > rrdjo.com.
  2. Netlify shows the DNS records to add. Add them where you bought
     rrdjo.com (or move the domain's name servers to Netlify).
  3. Netlify adds the secure https certificate automatically.
  Important: if rrdjo.com already handles your email (info@rrdjo.com),
  only add the website records Netlify lists. Don't delete your
  existing MX (email) records.

EDITING THE WEBSITE (any time)
  1. Go to  www.rrdjo.com/admin  and log in with GitHub.
  2. Open "All website content". Each section has English and Arabic boxes.
  3. Change text, add or remove products, countries, map cities or photos.
  4. Click "Publish" (top). The live site updates within about a minute.

GIVE A COLLEAGUE ACCESS
  They create a GitHub account. On GitHub open rrd-website > Settings >
  Collaborators > "Add people" and enter their username. Once they accept,
  they can log in at /admin.

STILL TO FILL IN (use the editor)
  Contact details > Address: replace "street address" with your office address.
