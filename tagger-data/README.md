# Corpora for tagger training

This folder contains the corpora required to train the statistical tagger. They are grouped in two folders, `tagged` and `crp`.

## tagged

Corpora for [supervised training](https://wiki.apertium.org/wiki/Supervised_tagger_training). Files must have the extension `.tagged` and each line must contain a disambiguated Apertium lexical unit, in [Apertium stream format](https://wiki.apertium.org/wiki/Apertium_stream_format). For example:

```
^Stelele/stea<n><f><pl><nom><def>$
^împodobesc/împodobi<vblex><pri><p3><pl>$
^cerul/cer<n><nt><sg><nom><def>$
^nocturn/nocturn<adj><mn><sg><nom><ind>$
^./.<sent>$ 
```

Before training, files from the folder are merged into a file named `ron.tagged`.

## crp

Corpora for [unsupervised training](https://wiki.apertium.org/wiki/Unsupervised_tagger_training). Files must have the extension `.txt` and contain **plain (raw)** text.

Before training, files from the folder are merged into a file named `ron.crp.txt`.
