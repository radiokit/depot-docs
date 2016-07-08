Getting Started
===============

RadioKit Depot repositories were designed for integration and centralization of
all of audio files needed for broadcasting and podcasting.

RadioKit approach lean to keep functionality of users as minimum,
and keep most of the settings separately, so you have to different "applications":
"Administration" and in case of Depot - "Library"

Repositories Administration
^^^^^^^^^^^^^^^^^^^^^^^^^^^

In Administration/File repositories you can manage your repositories functionalities,
check basic stats like "files count" or "total size", define its internal structure,
and of course create, delete or edit repositories itself.

After creating a repository, you can click on it and you'll get to a view with
tabs: metadata, tags, processors, imports, exports.


Metadata
********

Metadata is the place to keep whatever data about the file you need, or other
systems might need. So everything from a duration of file, through Idv3 tags, to
whatever custom data you would need - url links, replay gains, EbuR128 measurements,
comments etc.
Each metadata has its name, key and value type. Name can be changed flexibly,
however once key and value type are set, they can't be changed.

(note: for most of the use cases, there is one metadata field that should always
be created and never deleted - its field with the key "duration" and the same value type.)

Tags
****

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

Each file can be under unlimited number tags.
Tags are also base for automatic scheduling of broadcasting channels.


Processors
**********

Section processors is to define what kind of processes you want to apply to all
of your files in a repository - count its duration, generate waveforms, convert
to webformat, count replayGain, extract metadata from files. After you apply the
processor to the repository - the systems will be always searching for files, which
are lacking results of planned processes and in each case perform them.

Imports
*******

In this section you can define imports from your other systems, that will be
perform in 12h cycles - every 12 hours systems is going to check the differences
between your defined source, and your repository.

Export
******

In this section you can define exports to other systems (i.e. mixcloud),
where you want to publish your files.
Exports always takes files only from "Ready" tab of a repository.


Library
^^^^^^^

Upload
*******


After configuring your repository, you can go to the library and see the repository
actual workspace. You can start to upload your files (or there can already be some
if you defined import).

After clicking "Upload the files" you will see a modal for that process. You can
either drag&drop files on it, or click the button and choose the files from your
drive. When the upload is running you can close the modal and work in a repository,
but you can't leave or refresh the page as it will stop the upload.
You can see current stage of uploads either clicking on the small icon on the
top-right-corner, next to your login, or by clicking "upload files" once again.


(note:
It is advised to use "not to big" batches of files - few hundreds maxium.
Each files becomes a process in your webbrowser and they obviously act on this differently.
Google Chrome seems to be most effective.)


Tagging & Meta-dating;)
***********************

On the left side of your repository you see tree of tags, that you defined in
administration. Above files you see row with metadata you defined.

After you uploaded some files you should "Assign Tags" to each or all of them.

Depending on what metadata you defined in administration, what processors you
assigned to the repository, and what kind of metadata are written to the files
you have uploaded - most of the fields might become filled be itself. You can
give it a minute or two and refresh (if there is no upload ongoing), to see what its done.

Incoming, Ready, Archive, Trash
*******************************

The Tabs you see on the right corners tells you in which section you're at the moment,
You can move the files between the section, by checking the files and clicking
according button in the top-bar.


Workflow
********

The stage Incoming is the place, where you work with uploads (assinging tags &
metadata).
When your files are properly described, you can move them to "Ready".
"Ready" is the only stage that is "considered" by the systems, that make use of
repositories - its the place from where the Automatic scheduling takes files,
or the Chronicle seeks for podcasts.

When you want to put files aside you can keep them in "Archive" and when you think
they should be deleted, you can put them in "Trash", and either delete them, or
leave to someone who is responsible for exploring trashes.






.. toctree::
   :maxdepth: 2
