max-cube-protocol
=================

A attempt to write down the protocol of the eQ3 / ELV MAX! Heating system

This protocol is implemented in various opensource projects. To give an indication of the completeness of the implementation, a list of letters (Cube commands and messages), hexadecimal numbers (device radio commands), and more letters (Cube UDP commands) is provided. A project with a very short list might be an abandoned stub or written for a very specific use-case.

* [eq3-max](https://github.com/Juerd/eq3-max) (Perl) `ACLmMnNqsSt` 20, 22, 40, 82 `I`
* [FHEM](http://fhem.de/) (Perl) `aAcCHlLMnNrsStvx` 10, 11, 12, 20, 21, 22, 23, 30, 40, 42, 82, F0, F1
* [MAX_Boiler_Control](https://github.com/stephenmhall/MAX_Boiler_Control) (Python) `CHLM`
* [max-control](https://github.com/georg90/max-control) (NodeJS) `CHlLMsS` 40
* [MAXCPP](https://github.com/KnuthLohse/MAXCPP) (C) `CH`
* [maxcube](https://github.com/ivesdebruycker/maxcube) (Javascript) `ACHlLmMsS` 40
	* [mqtt-maxcube](https://github.com/leachj/mqtt-maxcube)
	* [maxcube-cli](https://github.com/ivesdebruycker/maxcube-cli)
	* [node-red-contrib-maxcube](https://github.com/ivesdebruycker/node-red-contrib-maxcube)
* [maxcube](https://github.com/aleszoulek/maxcube) (Python) `CHM`
* [Max::Cube](https://github.com/yoyostile/max-cube-ruby) (Ruby) `ClLq` - `hIN`
* [Max::Cube](https://github.com/joconcepts/max-cube) (Ruby) `H`
* [MAX-cube-ctl](https://github.com/pacostiro/MAX-cube-ctl) (C) `CHlLqs` 10, 11, 40
* [MAXDebug](https://github.com/bietiekay/hacs/tree/master/tools/MAXDebug) (C#) `HLM`
* [MaxManager](https://github.com/ababilone/maxmanager) (C#) `aACfFHlLMnNqsSu` 40 `I`
* [MAXSharp](https://github.com/bietiekay/MAXSharp/tree/master/MAXSharp) (C#) `HLM`
* [maxwindownotify](https://github.com/yfauser/maxwindownotify) (Python) `LM` - `I`
* [node-max](https://github.com/sebbo2002/node-max) (Javascript) `CHlL` - `I`
* [Openhab](http://openhab.org/) (Java)
	* [MAX! Binding](https://github.com/openhab/openhab2/tree/master/addons/binding/org.openhab.binding.max) `aAcCfFHlLmMnNqsStz` 11, 22, 23, 40 `chINR`
	* [maxcul binding](https://github.com/openhab/openhab/tree/master/bundles/binding/org.openhab.binding.maxcul) 00, 01, 02, 03, 10, 11, 12, 20, 21, 22, 23, 30, 40, 42, 43, 44, 50, 60, 70, 82, F0, F1
* [pymax](https://github.com/ercpe/pymax) (Python) `CfFHLMqsS` 10, 11, 12, 40 `IN`
* [thermeq3](https://github.com/autopower/thermeq3) (Arduino Yún) `CHLM`

General description on how to connect to the cube can be found in [protocol](protocol.md)

Info about discovery can be found  [here](Cube_Discovery.md)

Currently the following messages are described
* [A Message: Factory reset](A-Message.md)
* [C Message: Configuration](C-Message.md)
* [D Message: Decryption](C-Message.md)
* [E Message: Encryption](C-Message.md)
* [F Message: NTP server](F-Message.md) 
* [H Message: Hello](H-Message.md) 
* [L Message: Device List](L-Message.md)
* [M Message: Metadata](M-Message.md)
* [N Message: New device (pairing)](N-Message.md)
* [Q Message: Quit](Q-Message.md)
* [S Message: Send command](S-Message.md)
* [T Command: Delete device](T-Command.md)
* [U Message: URL configuration](U-Message.md)
* [Z Message: Wake up](Z-Message.md)

If you want to contribute, pull requests are welcome!
