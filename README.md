# MuST-Cinema
MuST-Cinema is a Multilingual Speech-to-Subtitles corpus built by annotating [MuST-C](https://ict.fbk.eu/must-c/) with subtitle breaks.
It comprises several hundred hours of audio recordings from English TED Talks, which are automatically aligned at the sentence level with their manual transcriptions and translations.
Special symbols have been inserted in the aligned sentences to mark subtitle breaks as follows:
- \<eob\>: block break (breaks between subtitle blocks)
- \<eol\>: line breaks (breaks between lines inside the same subtitle block)

Release v1.0: 7 language pairs
English to-{Dutch,French,German,Italian,Portuguese,Romanian,Spanish}

## Structure
### Data
The data is organised as follows:

Each folder (en-*target language) contains parallel data: train, dev and amara (test) as well as the corresponding yaml files containing the audio alignments.

The audio segments can be obtained from MuST-C. The same number of sentences has been preserved in MuST-Cinema.


### Docs
- MuST\_Cinema.pdf: LREC 2020 paper
- README.md: Description of the corpus


## Licence
TED talks are copyrighted by TED Conference LLC and licensed under a Creative Commons Attribution-NonCommercial-NoDerivs 4.0.

MuST-Cinema is released under the same Creative Commons Attribution-NonCommercial-NoDerivs 4.0 License.
