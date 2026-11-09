# App-All-O-Gizer

![App-All-O-Gizer's page, "Pronounced Apologizer", with an email address typed in and Send Email clicked, then a Gmail inbox opening an email from app.all.o.gizer titled "Sorry about the murder"](https://cloud.githubusercontent.com/assets/4650739/22124056/4d18bb72-de32-11e6-82ed-a89134d6c22c.gif)

*Pronounced Apologizer.* Sometimes you hurt people and don't even know it, so
the pitch was to apologize on a schedule and cover yourself either way. Type in
someone's email address, click Send Email, and they get one of 13 apologies
picked at random, from missing an anniversary to murder. I built it in a day at
the Stupid Shit No One In Hawaii Needs and Terrible Ideas Hackathon in January
2017.

[Read the full statement](https://www.joekarlsson.com/work/app-all-o-gizer/)

## Quick start

You need Node.js and a Gmail account with 2-Step Verification on, so you can
make a [Google App Password](https://support.google.com/accounts/answer/185833).
Gmail won't accept your normal password here.

```bash
git clone https://github.com/STUPIDSHITNOONEINHAWAIINEEDSHACKATHON/app-all-o-gizer.git
cd app-all-o-gizer
npm install
export email=YOUR_ADDRESS@gmail.com
export pass=YOUR_APP_PASSWORD
npm start    # open http://localhost:3000
```

## Development

The page is in `public/`, the send route is `routes/send.js`, and the
apologies are in `messages.js`. With `NODE_ENV=production` the server listens
on `$PORT`, and the `Procfile` runs `node server.js`.

## License

MIT. See [LICENSE](LICENSE).
