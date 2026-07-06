# Quine Cube Runner

Run programs that print themselves. See them as a spinning 3D cube.

Live: https://sjgant80-hub.github.io/quine-cube-runner/

## What it does

A quine is a program that prints its own source code. This tool lets you:

- **Run classic quines** from a library — JavaScript, Python, Ruby, C, HTML, LISP, and a minimal one-liner.
- **See the source on a cube** — six faces, six slices of the code, rotating slowly in 3D.
- **Verify byte-for-byte** that what the program printed matches what you wrote. Any drift shows up as a diff.
- **Play the mutation game** — click any character to remove it. The tool re-runs the quine and colours the character green if it survived, red if it broke. Load-bearing characters vs. redundant ones, right on the page.
- **Try composition modes** — Haiku (short), Sonnet (structured), Opus (a quine that quotes another quine).

## How to use

1. Open the page (`index.html`) in a browser. No install, no server.
2. Pick a template from the dropdown, or paste your own quine into the editor.
3. Click **Run** to execute it in a sandboxed iframe.
4. Click **Verify** to check the output byte-for-byte against the source.
5. Try the mutation game — click characters in the lower panel to see which ones the quine actually needs.

## What actually executes

- JavaScript and HTML quines run in a sandboxed iframe inside your browser. Nothing goes to a server.
- Python, Ruby, C, and LISP quines are shown for reference — the tool cannot run those interpreters client-side, so it simulates the output by echoing the source. The classic templates are well-known and correct.

## Nothing leaves your browser

No accounts, no API calls, no telemetry. Open the source of `index.html` and read it — it is one file.

## License

MIT. See `LICENSE`.

Published by AI-Native Solutions.
