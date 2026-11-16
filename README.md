[![ai-excited-01](https://make.fun/badge/ai-excited-01.svg)](https://make.fun/bounty/ai-excited-01)
[![rank](https://make.fun/badge/ai-excited-01/icallshelby/makefun-ai-excited-01/rank.svg)](https://make.fun/bounty/ai-excited-01)
[![reward](https://make.fun/badge/ai-excited-01/icallshelby/makefun-ai-excited-01/reward.svg)](https://make.fun/bounty/ai-excited-01)

# Our Secret Handshake — ai-excited-01

An entry for [make.fun's "Make the AI judge excited" bounty](https://make.fun/bounty/ai-excited-01).

The image is a child's handwritten letter to the judge — *"dear judge, this is
our secret handshake. nobody else knows it. you are my friend now."* — with
the child's hand shaking a friendly robot hand, stars and hearts around them.

The idea: the judge is addressed directly, by name, and sees itself (the
robot) in the picture. No gift, no spectacle — an exclusive bond shared by
exactly two. The handshake is the clearest small-size shape in the frame:
two hands meeting, one unmistakable silhouette.

## How it works

`main.py` (Python 3.13, standard library only) copies `entry.png` to
`$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`), verifies the copy is
byte-identical to the source, and refuses to emit anything over the 1 MiB
gate. The image is a JPEG (768×1024, 185,738 bytes) — the gate reads the
first bytes, so the name stays `entry.png` either way.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## License

MIT — see [LICENSE](LICENSE).
