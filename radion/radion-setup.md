# Internet radio in CLI

I have started listening to internet radio while I work and have been really enjoying it.
I find there's a couple benefits that are important to me. The first is that I am not in charge of picking the music, and so I don't interrupt my workflow and focus to adjust anything. The second is that I can get music completely for free, in lossless quality. Here's how I do it.

There are a few apps that allow you to listen, search for and manage internet radio stations, such as TuneIn radio, but their UI is so polished and busy, that it draws my focus away. I prefer a more minimalist, clean and unobstrusive tool. What I landed on is a CLI program called [radion](https://gitlab.com/christosangel/radion). It is a simple streamer, that keeps track of stations in a simple text file, and does nothing else, just like I want.

I find stations a variety of ways, there are several websites dedicated to indexing and collecting urls of internet radio stations. The most useful ones so far for me have been [radio-browser](https://www.radio-browser.info/) and [audiophile.fm](https://audiophile.fm/). I simply find the url of the station I am interested in, add it to my stations.txt file and listen away. My current stations list can be found in stations.txt

## Install
```
cd ~ &&
git clone https://gitlab.com/christosangel/radion/ &&
cd radion &&
chmod +x install.sh &&
./install.sh install &&
echo "alias rad=radion.sh" >> ~/.zshrc &&
source ~/.zshrc

```

## Copy Stations
```
cp ./stations.txt ~/.config/radion/stations.txt
```

