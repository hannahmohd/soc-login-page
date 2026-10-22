# soc-login-page
Browser-based SOC analyst login page with two-step verification and attempt lockout, built with Python (PyScript), HTML and CSS.
# Sentinel SOC Login

A login page for a security operations console, written in Python with PyScript. It runs entirely in the browser with no backend.

## Features
- Two-step sign-in: analyst ID and password, then a 6-digit verification code
- Lockout for 30 seconds after 3 failed attempts, with a live countdown
- Show/hide password button
- Enter key submits on every field
- Generic error message, so it doesn't reveal whether the username or the password was wrong
- Responsive layout with keyboard focus styles and screen-reader announcements

## Demo login
| Field | Value |
|-------|-------|
| Analyst ID | analyst01 |
| Password | Sentinel#2026 |
| Code | 123456 |

## Run it
Open `index.html` in a browser with internet access. PyScript is loaded from a CDN.

## Live demo
https://hannahmohd.github.io/soc-login-page/

## Limitations
This is a front-end demo. The credentials are in the page source and the lockout resets on refresh. A real system must verify passwords and one-time codes on a server.

## Built with
Python, PyScript, HTML, CSS
