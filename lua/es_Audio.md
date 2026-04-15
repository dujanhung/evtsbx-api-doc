<h2>
<code>es.Audio</code>
</h2>

<table><tr><td>
inherit
</td><td>
<code>es</code>
</td></tr></table>

a helper class to play audio files.

>[!IMPORTANT]
>"Evertech Sandbox" only support `WAV` file. other files would fire an error.

>[!TIP]
>if the file's source don't have `WAV` output, use file converter apps to convert them to `WAV` file.

>[!IMPORTANT]
>only one audio file could be played at the same block at the same time. trying to play the new one while the old one is still playing, would result in suddenly playing the new one instead.

>[!TIP]
>to play multiple audio files at a same time, you should create more blocks whose scripts are point to different audio files.
><h3>example</h3>
>block1
><codeblock lang="lua">
a
</codeblock>
>block2
><codeblock lang="lua">
a
</codeblock>

___

<h2>
property description
</h2>


