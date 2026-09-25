# Team Time

A lightweight, browser-based meeting activity for sharing team facts, starting guessing rounds, and viewing guesses in a live word cloud.

## Pages

- `team-time.html` is the presenter page. Add facts and names, choose the active fact, start a round, and review guesses.
- `team-time.html?view=participant` opens the participant view directly. Use the button at the top to switch back to presenter view.

## Run Locally

Open the `Team Time` folder in VS Code and serve it with a static web server, such as the Live Server extension. Open `team-time.html` in the browser.

## Publish with GitHub Pages

1. Add the contents of this folder to a GitHub repository.
2. In the repository, open **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the branch containing the files and the `/ (root)` folder, then save.
5. After GitHub Pages finishes deploying, open the site URL ending in `/team-time.html`.
6. Share the participant URL by adding `?view=participant` to that page URL.

For example:

```text
https://OWNER.github.io/REPOSITORY/team-time.html?view=participant
```

Replace `OWNER` and `REPOSITORY` with the GitHub account and repository names.

## Session and Privacy Limitations

This is a static, browser-only app. Session data is stored in that browser's local storage. It can be shared between pages in the same browser profile, but it does not synchronize across different browsers or devices. Participants opening the GitHub Pages URL on their own devices will not see or submit guesses to the presenter's session.

The presenter code only hides the presenter controls in the page. It is not server-side authentication and should not be treated as a security feature. Cross-device live sessions and secure presenter access require a shared backend and authentication.
