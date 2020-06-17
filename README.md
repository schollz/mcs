# mcs
MIDI chord sequencer, a fast and efficient way to send out MIDI patterns to multiple channels :musical_note:


<ul>
<li>There are 24 pulses per quarternote</li>
<li>Each measure has an adjustable number of quarter notes (2 - 4)</li>
<li>Each line is one measure</li>
<li>Each note cluster (notes with no spaces between) is subdivided into a measure equally, based on the number of note clusters (e.g. <code>CEG CEG</code> at <sup>4</sup>⁄<sub>4</sub> will be played for two beats each, and <code>CEG CEG CEG CEG</code> will be played for one beat each)</li>
<li>A non-note character indicates a rest (e.g. <code>CEG . CEG .</code> plays Cmaj on the 1st and 3rd beat)</li>
<li>A note cluster is non-separated list of notes and their octaves. If there is no octave information, the note chosen will be closest to the preceding note. (e.g. <code>C3B</code> will play <code>C3</code> and <code>B2</code>, while <code>C3B3</code> will play <code>C3</code> and <code>B3</code>).</li>
<li>A song is a group of measures (a set of lines). Each song will be transmitted to a MIDI channel.</li>
<li>Instruments are loaded in a separate area and can be assigned to any MIDI channel</li>
<li>Songs are saved</li>
</ul>