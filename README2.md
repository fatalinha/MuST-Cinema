# MuST-Cinema-PE
MuST-Cinema-PE is a corpus containing post-editing data of automatically-generated subtitles. It contains automatically-generated subtitles for 9 TED talk videos, their post-edited versions as well as process data (process logs, keystrokes) from three professional subtitlers in two language pairs (English into German/Italian). More details about the project can be found at https://mt.fbk.eu/must-cinema-pe/ .


## Structure
### Data
The 9 TED talks were split into 12 tasks of equal video duration. For en->it, 1,199 subtitles were collected for subtitler1 and 1,208 subtitles for subtitler2, while for en->de 1,198 subtitles. These correspond to 545 sentences for Italian and 542 sentences for German. The data is organised as follows:

- wav: the audio (.wav) files of the MuST-Cinema release (common for both language pairs).

For each language pair {de|it}:
- keystrokes: one log file for each of the 12 tasks as .csv files.

- log:  one log per subtitler containing all 12 tasks as .csv.

- srt: subtitle files (.srt) for each of the 9 talks for the system output (sys) and each post-editor {de|it1, it2}.

- txt: sentence-aligned .txt files consisting of the human source transcription (src), the target reference translation from TED (ref) and the .yaml files containing the audio alignment from MuST-Cinema, the subtitling system output (sys) and the PE versions by each subtitler {pe|pe1, pe2}. 


### Docs
- Subtitling guidelines.docx: File containing the subtitling guidelines and instructions given to the subtitlers
- Task questionnaire.csv: Post-task user experience questionnaire filled in by the subtitlers
- tasklist: File containing the number of the task, TED talk ID and link to video on the TED website
- Karakanta-etal-2024-Evaluating Automatic Subtitling.pdf: LREC 2024 paper describing the corpus and correlations of effort with MT metrics
- README.md: Description of the corpus


## Acknowledgements
This work was partially funded by the EAMT grant "2021 Sponsorship of Activities - Students’ edition" with the project title "Towards a methodology for evauating automatic subtitling". 

## Reference paper
If you use MuST-Cinema-PE in your work, please cite the following paper:

Alina Karakanta, Mauro Cettolo, Matteo Negri, Luisa Bentivogli. 2024. Evaluating Automatic Subtitling: Correlating Post-editing Effort and Automatic Metrics. In Proceeedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024), Torino, Italy, May 20-25 2024.