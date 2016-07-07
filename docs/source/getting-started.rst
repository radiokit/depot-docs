Getting Started
===============

RadioKit Depot repositories were designed for integration and centralization of
all of audio files needed for broadcasting and podcasting.

RadioKit approach lean to keep functionality of users as minimum,
and keep most of the settings separately.

Repositories Administration
^^^^^^^^^^^

In Administration/File repositories you can manage your repositories functionalities,
check basic stats like "files count" or "total size", define its internal structure,
and of course create, delete or edit repositories itself.

After creating a repository, you can click on it and you'll get to a view with
tabs: metadata, tags, processors, imports, exports.


Metadata
********************

Metadata is the place to keep whatever data about the file you need, or other
systems might need. So everything from a duration of file, through Idv3 tags, to
whatever custom data you would need - url links, replay gains, EbuR128 measurements,
comments etc.
Each metadata has its name, key and value type. Name can be changed flexibly,
however once key and value type are set, they can't be changed.

(note: for most of the use cases, there is one metadata field that should always
be created and never deleted - its field with the key "duration" and the same value type.)

Tags
********************

Tags' purpose is to label your files according to your needs, so you can navigate
through them and keep them in order you want.
Every single tag needs to belong to a group, which can have its own metadata schemas.
To make it more clear lets see possible use cases:
Group of Tags like:
Genre, Mood, Tempo,
could contain according tags, like:
Jazz, Rock, Blues;
Happy, Sad, Blue;
Fast, Slow, Stoner;
and so on, and so on.

Each file can be under unlimited tags.  


Processors
********************

Section processors is to define what kind of processes you want to apply to all
of your files in a repository - count its duration, generate waveforms, convert
to different format, count replayGain, extract metadata from files.






Workflow
^^^^^^^^

The workflow essentially looks like the following:




.. toctree::
   :maxdepth: 2
