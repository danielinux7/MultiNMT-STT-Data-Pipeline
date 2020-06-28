##### For data scientists, developers and whom it may concern: 
###### Some of the text materials are copyrighted, check out the multilingual sources section that links to the source, please be sure to obide the authors restrictions and limitations. Beside this, the repo is under CC0 (public domain) license. 
##### For copyright owners:
###### The text materials here are used for research, if there are any concerns regarding having your text material on this repo, please contact us via email(s): daniel.abzakh@gmail.com, kalle@hilsenbek.de.
##### Tools:
###### Composition of a training corpus
We can compose a specific training corpus and separate test files with the joined corpus script in the training directory:

    usage: join_corpus.py [-h] [--dictionary] [--numerate] [--paraphrase]
                          ll [ll ...] min_ratio max_ratio min_length max_words

    Process the corpus with paraphrases and the dictionary

    positional arguments:
      ll            the lengths for dictionary lists
      min_ratio     We only use translations with this minimum, parallel ratio
      max_ratio     We only use translations with this maximum, parallel ratio
      min_length    We only use translations with this minimum length
      max_words     We only use translations with this maximum words

    optional arguments:
      --dictionary  We use the dictionary as translation source
      --numerate    The dictionary list has a numeration
      --paraphrase  We paraphrase the filtered corpus

For example `python3 join_corpus.py --dictionary --paraphrase 1 0.7 2.25 10 50` results in the commited `06-19-2020_corpus` with a minimum range of 10 letters, max 50 words, a min ratio of 0,7 and max ratio of 2.25. The paraphrases are based on the filtered, training copus and are joined with the plain dictionary.
#### Current Multilingual Corpuses:
1. Abkhazian Russian Parallel corpus (~121k lines).
#### Multilingual sources:
-	100 text book: http://apsua.tk/upload/iblock/54c/54cfde81abd369cdffa6512d9fdbea1e.pdf
-   Declaration of Human Rights: https://www.ohchr.org/EN/UDHR/Documents/UDHR_Translations/abk.pdf
-	Braveheart: https://www.opensubtitles.org/en/subtitles/7977089/braveheart-ab
-	The new testament book: http://apsnyteka.org/3009-Novy_zavet_2015_abh.html
-	Abaza site articles: http://abaza.org/
-   Apsnypress articles: http://apsnypress.info/
-   Tatoeba: https://tatoeba.org/eng/sentences/search?query=&from=rus&to=abk
-   JW: https://wol.jw.org/
-   JW300: http://opus.nlpl.eu/JW300.php
-   Constitution: https://ru.wikipedia.org/wiki/Конституция_Республики_Абхазия
-   Criminal codex: http://presidentofabkhazia.org/doc/codecs/
-   Family codex: http://presidentofabkhazia.org/doc/codecs/
-   Quran: https://github.com/danielinux7/Abkhazian-books-in-Public-Domain/tree/master/Аҟәырҟан
-   The president's cat: (Одишариа, Гәырам: Апрезидент ицгәы) http://clarino.uib.no/abnc/text-list
#### Further resources
- https://github.com/christos-c/bible-corpus
- A Review of Past Work and Future Challenges https://arxiv.org/pdf/2006.07264.pdf
- Tools and resources for open translation services: https://github.com/Helsinki-NLP/Opus-MT
- https://paperswithcode.com/task/low-resource-neural-machine-translation
- https://www.masakhane.io/ https://github.com/masakhane-io/masakhane/blob/master/MT4LRL.md low resource, african NMT
- https://glosbe.com/ab/ru/ multilingual dictionary api
- https://babelnet.org/ multilingual semantic network
- https://iconictranslation.com/2020/02/sequence-to-sequence-pre-training-for-neural-mt/
- Research for paraphrasing in NMT:
  https://www.aclweb.org/anthology/W17-5703.pdf
  https://iconictranslation.com/2020/02/issue-69-using-paraphrases-in-multilingual-neural-mt/
