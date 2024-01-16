# VideoQueue2Markdown

(What does it say about someone when the first two projects they make in C++ have to do with organizing files? Am I working my way towards being the Marie Kondo of software? Or am I just sort of neurotic about my file management? I'm not sure.)

Regardless of what it reflects about my psyche, VideoQueue2Markdown (VQ2M) is a C++ app that makes it really easy to make a queue for watching videos you have downloaded, provided you have my specific workflow. 

Simply compile the .cpp file and run the output in the directory where you have lots of videos stored. For example, let's say that you have a bunch of DVDs (lol) which you have ripped into a directory called `MyShows` that looks like this:
```
MyShows/
│
├── Oregairu/
│   ├── Season 1/
│   │   ├── Oregairu S01E01.mp4
│   │   ├── Oregairu S01E02.mp4
│   │   └── Oregairu S01E03.mp4
│   │
│   └── Season 2/
│       ├── Oregairu S02E01.mp4
│       ├── Oregairu S02E02.mp4
│       └── Oregairu S02E03.mp4
│
└── Steins;Gate 0/
    ├── Steins;Gate 0 E01.mp4
    ├── Steins;Gate 0 E02.mp4
    └── Steins;Gate 0 E03.mp4
```

After navigating to the directory and running VQ2M, it will recursively trace through all of the subdirectories and generate a Markdown file with headers for each subdirectory and convenient checkboxes next to each episode of your ~~weeb shi~~ high quality entertainment, making it easy to mark what you have or haven't watched. So after running VQ2M in `MyShows/`, you would get a markdown file called `video_queue.md` that looks like this:

```
# Oregairu
- [ ] Oregairu S01E01
- [ ] Oregairu S01E02
- [ ] Oregairu S01E03
- [ ] Oregairu S02E01
- [ ] Oregairu S02E02
- [ ] Oregairu S02E03

# Steins;Gate 0
- [ ] Steins;Gate 0 E01
- [ ] Steins;Gate 0 E02
- [ ] Steins;Gate 0 E03
```
After that, you can open the .md file in any Markdown editor (I like Obsidian) and easily mark which episodes you've watched, making it considerably easier to manage all of the videos you want to watch.
