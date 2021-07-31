# Efabless-Contest-Serial RISC V (SERV)

## Guide:
### Mr.K.Radha Krishnan

## Team Members:
 
 ### A.John Samuel Ebenezer(Lead Designer)
 ### R.Thanga Gnana Jenef
 ### G.Shri Hari
 
 
 ## Description:
 SERV is a bit-serial CPU which means that the internal datapath is one bit wide. SERV internal dataflow show the internal dataflow. For each instruction, data is read from the register file or the immediate fields of the instruction word and the result of the operation is stored back into the register file. Reading and writing memory is handled through the memory interface module.
 
 ![serv_dataflow](https://user-images.githubusercontent.com/61493308/127742606-6aa31a10-4b3b-466b-8cd0-4b6f29fad512.png)
 
 ## Performance Comparision:  
 
 
 
    Core		      LUT	  FF	   DSP	 BRAM	IPC	  MFreq	     Ncores	  MIPS/k7	
	  DarkRISCV	      1177	246	   0	    0	   1	   150	     221	    33232	
	  VexRISCV	      1993	1345	  4	    5	   1	   214	    130	       28013	
	  PicoRV32	      1291	568	   0	    1	  1/4	   309	    201	       15630	
	  SERV		         217	174	   0	    0	 1/32	   367	   1200	       13788
	  RPU		          2943	1103	  12	   1	   1	   111	    88	      9905	
    UE RISC-V	      3676	2289	   4	   0	   1	   124	    70	      8811	
    UE BiRISC-V            15667	6324    4	   0	   2	    87	     16	      2917	
     
 

 ## Design Goals:
 1) Applications have to be preloaded to RAM at compile-time
 2) Make it faster and smaller
 
