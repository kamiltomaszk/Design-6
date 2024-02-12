# Lab 1 — GHDL and GTKWave
Very High-Speed Integrated Circuit Hardware Description Language (VHDL) is a programming language used to model digital models.
G Hardware Design Language (GHDL) is an open-source simulator, compiler, and VHDL analyzer for the VHDL language. The G has no meaning.
## Installing GHDL and GTKWave
To start using VHDL, I followed the tutorial ['Getting Started With VHDL on Windows (GHDL & GTKWave)'](https://www.youtube.com/watch?v=H2GyAIYwZbw) by Nerdy Wave.
After installing GHDL and GTKWave, I ran my first 'Hello, World' using GHDL to make sure it was working correctly.

## Half Adder
```
$ ghdl -a ha.vhdl  
$ ghdl -a ha_tb.vhdl  
$ ghdl -e ha_tb  
$ ghdl -r ha_tb --vcd=ha.vcd  
ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test  
$ gtkwave ha.vcd  
```
![](half_adder.png)

## D Flip-Flop
```
$ ghdl -a dff.vhdl
$ ghdl -a dff_tb.vhdl
$ ghdl -e dff_tb
$ ghdl -r dff_tb --vcd=dff.vcd
$ gtkwave dff.vcd
```
![](d_flip_flop.png)
