# LinkedIn Roulette 🎡

A silly 90s-game-show-style web app for reconnecting with your LinkedIn network.

Load your `Connections.csv`, spin the wheel, and get challenged to reach out to a random connection with a prompt like **THROWBACK**, **CONGRATS**, or **GOSSIP**.

## How to play

1. Open `index.html` in a browser. It's a single file with no build step or install.
2. Load your `Connections.csv` (see below for how to get it).
3. Optionally filter by job title, company, or the year you connected.
4. Hit **SPIN!** The marquee picks your mystery guest and the wheel picks your challenge.
5. Reach out, then click **I did it! 🎉** to add them to the **Hall of Fame**. Or click **Chicken out 🐔**, enjoy the chicken rain, and they land in the **Chickens of Shame** (you can redeem yourself later).

To try it without your own data, load `sample-connections.csv`.

## Getting your Connections.csv

1. On LinkedIn, go to **Settings & Privacy → Data privacy → Get a copy of your data**.
2. Choose **Connections** and request the archive.
3. When LinkedIn emails you, download and unzip it. The file you want is `Connections.csv`.

## Privacy

Your file is read entirely in your browser. Nothing is uploaded, sent anywhere, or saved, not even to browser storage. Closing or refreshing the tab clears everything. Use **Copy** or **Download CSV** in the Hall of Fame if you want to keep your list.

## Customizing the challenges

The wheel's challenges live in the `WEDGES` list in `index.html`. Each one has a short `label` (about 12 characters max, so it fits on a wedge) and a `tpl` prompt. Prompts can use these placeholders:

- `{first}`: the person's first name
- `{company}`: their company
- `{aPosition}`: their job title with "a" or "an" in front
- `{yearsPhrase}`: how long you've been connected, like "3 years"

---

Made for fun. Not affiliated with LinkedIn.
