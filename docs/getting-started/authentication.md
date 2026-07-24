# Logging In

There are two ways to log in to the staging site: an **email account** created for you by an admin, or an **ORCID sandbox account**. Which one you use depends on what access you've been given.

## Starting the login process

From any page, click **LOGIN / REGISTER** in the top-right corner.

![Top banner before login](../assets/screenshots/auth/top-banner-before-login.png)

You'll be taken to the sign-in screen:

![Sign in screen](../assets/screenshots/auth/login-screen-first.png)

From here you can either sign in directly with a username/email and password, or continue with ORCID.

## Option 1: Email login (by invitation only)

On staging, email/password accounts are **not self-service** — an administrator has to pre-create an account for your email address before you can sign in this way. If you haven't been given an account and password, use the ORCID option below instead, or contact an admin (see [Support](../reference/support.md)).

## Option 2: ORCID login (sandbox)

Most staging users authenticate via ORCID. This comes with one important catch:

!!! warning "Staging uses ORCID *sandbox*, not your real ORCID account"
    Because this is a test/staging environment, it is wired up to ORCID's **sandbox** system (`sandbox.orcid.org`) rather than the real, production `orcid.org`. Your normal ORCID iD and password will **not** work here — you need a **separate sandbox ORCID account**.

**Before you log in for the first time**, it's easiest to create your sandbox ORCID account ahead of time:

1. Go to [sandbox.orcid.org](https://sandbox.orcid.org/) and register for a sandbox account, just as you would on the real ORCID site.
2. Keep the sandbox email/password somewhere safe — it's unrelated to your real ORCID credentials.

Then, on the staging sign-in screen, click **ORCID**. If you haven't pre-created a sandbox account, you'll land on the ORCID sandbox sign-in/registration page and can register from there instead:

![ORCID sandbox sign-in](../assets/screenshots/auth/login-orcid-sandbox.png)

Note the yellow banner confirming you're on `sandbox.orcid.org` — a test website that only sends email to `mailinator.com` addresses. This is expected and only appears because this is the staging deployment.

Once you sign in through ORCID sandbox, you're redirected back to the site, already logged in.

## After logging in

Once authenticated, the top banner shows your name and a **LOGOUT** option instead of **LOGIN / REGISTER**:

![Logged in, top banner](../assets/screenshots/auth/logged-in-closeup.png)

![Logged in, full page](../assets/screenshots/auth/home-after-login.png)

Clicking **LOGOUT** ends your session and returns you to the logged-out home screen.
