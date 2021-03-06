# microbench
Extremely Simple Microbenchmarks

To build X86 binaries,  
```shell
make
```

To build ARM binaries,
```shell
make ARM
```

To build RISCV binaries,
```shell
make RISCV
```

To build X86, ARM, and RISCV binaries,
```shell
make all
```

To set the path to X86 compiler, change `$CC_X86` in `make.config` file.  
To set the path to ARM compiler, change `$CC_ARM` in `make.config` file.  
To set the path to RISCV compiler, change `$CC_RISCV` in `make.config` file.  

The binaries are named `bench.X86`, `bench.ARM`, and `bench.RISCV` on each subdirectory.

From the original README file,

> Hi,
> 
> This is an *extremely* simple microbenchmark suite.
> 
> Its intended purpose is in the validation of general purpose out-of-order  
> cores, by targetting individual micro-architectural features or effects.  
> Of course this is by no means an exhaustive collection of necessary bencharks  
> to test every mechanism in an OOO processor.  This is merely a starting point.  
> 
> To use this, you should only need bash, make and python.  
> 
> Configure the versions of the compiler and python (tested with python-2.7):  
> > vim make.config
> 
> To make the benchmarks:  
> > make
> 
> Clean the benchmarks:  
> > make clean
> 
> Describe basically what each benchmark is for:  
> > describe.sh
> 
> Run a benchmark: (no args on any current benchmark)  
> > cd CCa  
> > ./test
> 
> Tony Nowatzki  
> Tuesday, April 14th, 2015  
> 
> PS: Also, some benchmarks use an LFSR setting to get a particular working set.  
> Please see lfsr_settings.txt for example values. (bench ML2 uses this)  
