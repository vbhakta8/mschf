# Future - Crawler ft. Lil Uzi Vert
Small Project to try and crawl the highoff pages

[mschf](https://www.mschf.xyz) release a project in collaboration with Future. This crawler will help you find the right page the song is on.

On MacOS be sure to install the chrome webdriver.

Best way I have found is using [brew](https://brew.sh/)
```
brew cask install chromedriver
```

```
virtualenv -p python3 env
source env/bin/activate
pip install -r requirements.txt

python mschf.py
```

In the commandline you will be given the url with the current active playing session. Each session last 10 minutes before moving to a new domain.

With some digging if you wanted to download the `*.mp3` file they are streaming you can just pop open your develop tools and go to the `network` tab and find the request being made.

I have already done this, [here is where the file is stored in S3](https://s3.amazonaws.com/highoff.life/computer-virus-do-not-click.mp3). Quarantine got me real bored, so I hope you found this useful.
