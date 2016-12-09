# text-fabric-data

![text-fabric](https://raw.github.com/ETCBC/text-fabric/master/docs/tf.png)

Textual data of ancient sources to be used in conjunction with
[Text-Fabric](https://github.com/ETCBC/text-fabric)

# Available data sources

## Hebrew

### etcbc4c

Hebrew Text Database, text and linguistic annotations made by the
[Eep Talstra Centre for Bible and Computer](http://www.godgeleerdheid.vu.nl/en/research/institutes-and-centres/eep-talstra-centre-for-bible-and-computer/index.aspx)
and prepared for online use and use in Text-Fabric by Dirk Roorda
[Data Archiving and Networked Services](https://dans.knaw.nl/en/front-page?set_language=en)

This source a follow-up version of **etcbc4b**, which is documented on 
[SHEBANQ](https://shebanq.ancient-data.org/sources).

The same license conditions apply.

**etcbc4c** has been compiled by means of
[tfFromLAF](https://github.com/ETCBC/text-fabric/blob/master/tfFromLAF/tfFromLAF.ipynb).

### phono

Phonetic transcription of the text in the **etcbc4c** database.
The transcription is algorithmically produced by a notebook that makes use of the corpus as whole.
The notebook provides the result as a *module* to the **etcbc4c** core data.
As such it can be seamlessly imported by Text-Fabric.
