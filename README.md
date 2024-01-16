# VideoQueue2Markdown

What does it say about someone when the first two projects they make in C++ have to do with organizing files?

VideoQueue2Markdown (VQ2M) is a C++ app that makes it really easy to make a queue for watching videos you have downloaded, provided you have my specific workflow. 

Simply compile it the .cpp file and run its output in the directory where you have lots of videos stored. For example, if you ripped the files off of some DVDs or something like that (lol) and have them stored inside of one directory, you would go inside of that one directory and run VQ2M. After that, it will recursively trace through all of the subdirectories and generate a Markdown file with headers for each subdirectory and convenient checkboxes next to each episode/file, making it easy to mark what you have or haven't watched. For example, let's say that you store your ~~weeb~~ high quality entertainment in a directory called "MyShows" that looks like this:

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

After running VQ2M, you would get a markdown file called `video_queue.md` that looks like this:

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
