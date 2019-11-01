## **Nodes**

  Tap anywhere in the big circle to add a node. Each node represents a sound or a MIDI note, with the color of the node controlling which sampler / channel the node uses.

  The closer a node is to the middle, the faster it will repeat.

  ---

#### **Node Parameters**
  The buttons around the big circle represent different parameters that can be applied to each node. Each half of the big circle is a slider that is used to change these node parameters.

  See the quick reference (the question mark button in the menu bar) for a description of what each parameter does.

  **Double tap** a parameter button to reset that parameter for all nodes. **Long pressing** a button will reset that parameter for the selected colors nodes only.

  ---

#### **Randomising Nodes**
  The controls to the right of the node screen can dramatically affect the the sound of Poly. These controls can randomise the position and color of the nodes, as well as randomising the selected parameter for each node. **Tapping and holding** the randomise parameter button will apply the effect to the selected colors nodes only.

  When the position and color of the nodes is in a randomised state a plus icon will appear to the left of the button. **Sliding your finger over to this button will copy the randomised nodes to a new pattern.**

## **The Grid**
  The playback position of each node is determined by its position on the grid. Each subdivision starts from 12 o'clock and works clockwise.

  For instance, the 4th ring from the middle has 4 positions and the first position to play starts at 12 o'clock. This node will play again after 4 pulses, with the length of a pulse being determined by the patterns quantise settings.

  You can have more than one node on a single position.

  Use the **Grid Icon** on the left of the node screen to turn the grid on and off.

## **Patterns**

  The pattern menu can be found by toggling the **Pattern Button** in the bottom right corner of the node view. These patterns represent different configurations of nodes.

  You can have up to 16 different patterns for any project.

  On the left you can find the controls for each pattern, whilst on the right you can find the controls for selecting different patterns. There is a **Quick Copy** button above the pattern selectors which will copy the current pattern to the next available pattern, without stopping playback.

  ---

#### **Pattern Editing**
  Patterns can be copied and pasted between each other using the buttons on the left of the pattern menu. There is also a clear button for removing all the nodes from a pattern.

  **It is also possible to paste and clear only the selected colors nodes.** This is achieved the same way as randomising / resetting the selected colors node parameters, by long pressing the paste and clear buttons. The copy button will always copy the whole pattern. This allows you to perform edits to specific colors of nodes without having to alter a whole pattern.
  ---
#### **Pattern FX**
  There are 4 FX configurations available for each pattern to choose from. These FX slots can be populated from the FX page. Each pattern can store an FX slot and upon changing to that pattern, the corresponding FX configuration will be selected.

## **Keyboard**
  Each node will select its pitch based on the keyboard. There are three modes a keyboard can be set to: **Random, Sequence and MIDI**.

  ---
#### **Random Mode**
  Each node will select a pitch from the selected keys at random everytime it plays.
  ---
#### **Sequence Mode**
  Each node will select the next pitch in the sequence. Once a pitch has been selected, the sequence moves on to the next step and the next time a node plays it will select that pitch.
  ---
#### **MIDI Mode**
  The keyboards selected pitches are controlled via **external MIDI**. Note on messages cause a pitch to be selected, whilst note off messages remove that pitch. The keyboard is locked to 2 octaves, but you can use any 2 consecutive octaves to control it.

  You can optionally choose to apply the note ons velocity to the node as well, although this will override the velocity settings that come from Poly. See the **Keyboard** section of the **MIDI settings menu** to configure this.

## **Sampler**

  This is where you can control the sound that is produced by each color. All samplers have 8 voices of polyphony, but can be set to mono mode for sounds with lots of bass.
  ---
#### **Loading Sounds**
  Sounds can be loaded into the sampler by **tapping on the waveform**. This will display the sound selection menu. From here you can load a new sample into the sampler, or you can load a collection of sounds (a kit) into all samplers.

  **Custom kits can be saved from within the Kits menu.**
  ---
#### **LFO**
  The LFO is a constant rate from the moment the sequencer starts. This means it does not retrigger with each sound.
  ---
#### **Sample Offsets**
  Each samples start and end points can be adjusted by using the markers on the waveform. These end points also determine the loop points for that sample.
  ---
#### **Copy and Paste**
  Samplers can be copied and pasted between each other. It's possible to paste just a samplers settings, without pasting the audio file.
  ---
#### **Crossfading**
  Looping samples can have a crossfade effect applied to them. This is useful for smoothing out any clicks that can be caused by having a loop point on a non zero crossing. It also allows you to create pad sounds out of any audio sample.
  ---
#### **Envelope Length**
  The envelope lengths (attack, sustain, release) are displayed as a maximum value. However, **a node can alter this using it's own length parameter.** For example, if a node has a length of 50%, all the envelopes settings will be halved.  

## **FX**
  These are the global FX settings for each project. The delay and reverb are send effects, whilst the distortion and EQ are global effects. The four configurations can be assigned to individual patterns.

  The FX chain is *Sends > Distortion > EQ*

## **Mixer**
  These are the mixer settings for each sampler. There is a limiter at the very end of the processing chain to prevent overloading. A small red dot will appear next to the master level knob to show when the limiter is taking effect. The master level can be used as the input gain for the limiter.

## **MIDI**
  Poly supports external, network and virtual MIDI. Note, velocity and CC events can be both sent and received, whilst clock messages can only be received.
  ---
#### **Track Out**
  Each color can be configured to send events to a specific MIDI destination and channel. CC message and notes can be enabled or disabled here. If you want a color to only send MIDI, you can disable audio processing from here too.

  The length of a MIDI note is set to it's maximum here. The actual length can be adjusted on a per node basis, using the length parameter of that node.
  ---
#### **Keyboard**
  These are the controls for each colors keyboard when it is MIDI mode. If velocity is enabled, the velocity of each note in will be applied to the node that selects it. This will override the nodes own velocity setting.
  ---
#### **Node MIDI CC Out**
  Nodes can be configured to send CC out messages. Each node parameter can be assigned a MIDI CC number and will send an event between 0 - 127, depending on the parameter value for that node.

  For assigning external controls to Poly's CC out messages, you can activate MIDI Learn mode from the transport and then **double tap the node parameter button**. This will send a CC message to any connected receivers.
  Use the **Track Out** menu to configure the destination for CC messages.
  ---
#### **MIDI Learn**
  Some controls in Poly can be assigned to receive MIDI CC messages. Activate MIDI learn mode from the transport bar and all assignable controls will now show a plus icon. When the icon is red, that means a control is ready to be assigned, when it is green it means it has already been assigned. A white icon means the control is in a neutral state.
  ---
#### **Importing MIDI Configurations**
  MIDI settings in Poly are saved on a per project basis. However, a projects settings can be imported to any new project using the **Import** button in the MIDI menu.

## **Managing Files and Importing Audio**
  The **Files** menu can be used to import audio from either the iOS Files app or the browser based WIFI transfer. WIFI transfer is great for getting files from your desktop into Poly.

## **Performance**
  You can change some of the apps behaviour from here. 
  ---
#### **Use Pattern FX** ####
  Using the pattern FX will mean that when a pattern is selected, the patterns FX configuraton will also be selected. Otherwise, the configuration remains the same when the pattern is changed.
  ---
#### **Quantise note lengths** ####
  A nodes length will be quantised to a multiple of 8. So 12.5%, 25%, 37.5% etc. This is good for creating exact multiples of length and works very well with tempo synced MIDI note lengths.
