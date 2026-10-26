# SoundAlike

Pick a song, and SoundAlike finds the songs that sound most similar to it.

This is our final project for CSC 212 (Data Structures and Abstractions) at the University of Rhode Island, Fall 2026.

**Team:** Daniel Linde, Kevin Chen

## What it does

Each song in our dataset is described by a few numbers, like energy, danceability, tempo, and how happy it sounds. We treat every song as a point in space, so songs that are close together sound alike.

To find the closest songs quickly, we built a **k-d tree** in C++. We compare it against a brute-force search that checks every song, and measure how much faster the tree is as the library grows.

## Project status

🚧 In progress. Planned milestones:

- [ ] Choose and clean the song dataset
- [ ] Brute-force search (baseline)
- [ ] k-d tree: build and nearest-song search
- [ ] Tests comparing the k-d tree to brute force
- [ ] Benchmarks and plots
- [ ] Interface for searching songs

## Repository layout

```
src/          C++ source code (k-d tree, brute-force search)
tests/        Correctness tests
benchmarks/   Timing experiments and plotting scripts
data/         Song dataset (see "Data" below)
```

## How to build and run

_Coming soon. We'll add the exact commands once the first version runs._

Requirements so far:

- A C++17 compiler (e.g., `g++`)
- Python 3 (for data preparation and the interface)

## Example

_Coming soon._ It will look something like this:

```
Search for a song: Blinding Lights

10 most similar songs:
  1. ...
  2. ...

k-d tree search:     0.2 ms
Brute-force search:  45.0 ms
```

## Data

We use a public song dataset from Kaggle that lists audio features for each song. _Link and download instructions coming soon._

## Report

Our full report, including design, analysis, and benchmark results, will be in [REPORT.md](REPORT.md).
