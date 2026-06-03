# base64copier
Base64Copier is a simple tool to copy and paste files between different environments, where files as such cannot be transferred directly.

Here are the links to the artefacts for your convenience:
- [Link to artefact #1](index-01.html)
- [Link to artefact #2](index-02.html)

### Motivation
The need for the tool was suddenly realized as a binary file (.pdf) needed to be transferred between systems that only allowed text mode copy & pasting. Then, Generative AI (GenAI) was utilized to produce a minimal viable product (MVP) to realize that need.

The secondary purpose was to demonstrate whether GenAI can produce an acceptable artefact if/when the user knows exactly what they want and need.

Created with assistance of Copilot Think Deeper mode on 2026-06-03 in about 15 minutes.

### Prompts
1. `make very simple html5 website that1) encodes uploaded file as base64, user can copy2) allows download of a base64 encoded file, user can paste3) works completely on browser, ie no networking required`
<-- Begins to respond with a React based solution, which is stopped as too complicated for request
2. `no no, don't use react or such compilable framework, resort to pure html5 and javascript`
<-- Reasoning completed in 1 step and produces a plain HTML, CSS and JavaScript website
3. `is there a maximum amount of copy&paste buffer in for example tigervnc?`
<-- Reasoning completed in 7 steps and answers as questioned, only about tigervnc
4. `linux cli tool to cut 256kb from a file`
<-- Reasoning completed in 1 step and gives a few options to do chunking
5. `ok, update the website with optional chunking strategy, so that on encode side user may specify the size of chunks in KiBs, by default 255, then on decode side user may choose amount of chunks and website will provide pasteable text areas as requested`
<-- Reasoning completed in 1 step and produces another standalone and more stylished webpage

### Iterations & Artefacts
#### Iteration "0"
Summary: Result of the prompt #1 was discarded already during the generation because of too not matching with the requirements.

The initial attempt to generate the MVP, however, GenAI model was rather too eager to produce more sophisticated framework than what was required.

#### Iteration 1
Summary: Result of the prompt #2 can be considered as the first proper artefact. The artefact was a rudimentary tool which fulfilled its required task and nothing more.

The first real MVP came from this iteration as the model was instructed to step back and generate more simple artefact. [Link to artefact #1](index-01.html)

#### Iteration 2
Summary: Result of the prompt #5 can be considered as the second artefact. The artefact was more polished version with additional features that were discovered after the first artefact was produced.

The second MVP was an incremental improvement to the first due to a change in the requirements. While manual cutting of the Base64 string is possible, this iteration added the quality-of-life improvement to cut and stitch chunks more intuitively. [Link to artefact #2](index-02.html)
