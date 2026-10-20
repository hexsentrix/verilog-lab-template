# verilog-lab-template

This 

## Usage:

Compile and run

```
mkdir -p waves
iverilog -g2012 -Wall \
  -s project_tb \
  -o /tmp/project_sim \
  src/project.v tb/project_tb.v
vvp /tmp/project_sim
```

## Validation:
```
verilator --lint-only -Wall src/project.v
```