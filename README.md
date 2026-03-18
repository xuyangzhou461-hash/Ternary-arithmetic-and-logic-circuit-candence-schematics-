# Compatibility Warning
**You need**: tsmc18rf technology library, Stanford CNFET models, Cadence Virtuoso

The STI designs and TNAND schematic designs require only the two CNFET models and are the most likely to be portable. 
The THA designs required additional binary gates and are not portable since they needed extra binary gates!!!
The exact parameters (n,m) for each CNFET are not provided.

# Report gist
This repository is an extension to the "Is Ternary Computing more Efficient than Binary?" passion project and contains a complete suite of ternary and binary logic circuits, including personal optimizations and recreations of existing work. Multiple variations of ternary logic gates were assembled and verified via transient analysis. The key findings of this passion project include:

1. **Logic Gate Speed & Power:** 32nm CNTFET ternary gates (TNAND and STI) operate with delay in the femtosecond ($10^{-15}$) range and consume power in the nanowatt ($10^{-9}$) range, significantly outperforming 180nm CMOS binary equivalents.
2. **Arithmetic Efficiency:** The proposed THA design demonstrated extraordinarily high energy efficiency, consuming only 1.274 $\mu W$, outperforming the 180nm binary half adder in power usage.
3. **Interconnect Reduction:** Due to higher information density, ternary systems require fewer physical wires. For example, representing 32 states requires 5 binary bits but only 3 ternary trits, resulting in a 66.7% reduction in wires.


# Repository Contents:
Circuit schematics for Ternary Half Adders (THA), Ternary NAND (TNAND), Ternary NOR (TNOR), and Standard Ternary Inverters (STI).

**Simulation Software:** Cadence Virtuoso and Spectre.

**Transistor Model:** Stanford University Carbon Nanotube Field-Effect Transistor (CNFET) Model. 

**Binary Benchmark:** tsmc 18rf technology library (180 nm CMOS).

### STI Gate

*STI Saketh*
<img width="1758" height="1401" alt="STI_Saketh_inner" src="https://github.com/user-attachments/assets/bcddb95f-6876-4971-82e2-6e2f9a27a13a" />

*STI Jaber*
<img width="1738" height="1038" alt="STI_Jaber_inner" src="https://github.com/user-attachments/assets/cb1158dc-ebcc-43dc-ba90-82cb48f2cc62" />

*STI Lin*
<img width="1199" height="1416" alt="STI_Lin_schematic" src="https://github.com/user-attachments/assets/aba66fa0-4351-4acf-a6cb-6dcd35baaad0" />

*STI trans Graph*
[STI_Jaber_trans_thick.pdf](https://github.com/user-attachments/files/26088434/STI_Jaber_trans_thick.pdf)


### TNAND Gate
*TNAND Jaber*
<img width="1916" height="1390" alt="TNAND_Jaber_withsubcircuits" src="https://github.com/user-attachments/assets/52cdd6b9-9421-4b59-ad3f-7bc7d230056b" />

*TNAND Lin*
<img width="1631" height="1392" alt="TNAND_Lin_schematic" src="https://github.com/user-attachments/assets/d1d6a989-e646-4c4e-823e-4c76e70b385d" />

### Tdecoder
*TDecoder Jaber*
<img width="1480" height="1022" alt="Tdecoder_Jaber_inner_schematic" src="https://github.com/user-attachments/assets/34004679-c405-41f1-a4e4-8fcea04c50b0" />


*TDecoder Lin*
<img width="1479" height="1022" alt="Tdecoder_Lin_schematic" src="https://github.com/user-attachments/assets/02c5f0d8-1e30-484e-942e-df41e486be14" />

*TDecoder Graph*
[Tdecoder_Jaber_graph.pdf](https://github.com/user-attachments/files/26089655/Tdecoder_Jaber_graph.pdf)

### Ternary Half Adder
*THA Lin*
<img width="1155" height="1414" alt="THA_Lin_schematic" src="https://github.com/user-attachments/assets/c0ce0d91-5d81-4cb7-ab5a-0d01d7c1f8cc" />

*THA Jaber*
<img width="1480" height="1022" alt="THA_Jaber_schematic" src="https://github.com/user-attachments/assets/5a9960d9-f27c-4009-906f-69df29f40883" />

*proposed THA*
<img width="1255" height="1361" alt="proposed_THA" src="https://github.com/user-attachments/assets/0912dc43-8eef-49bc-8d2b-ac70f42029f7" />
[proposed_THA_graph.pdf](https://github.com/user-attachments/files/26088440/proposed_THA_graph.pdf)

*TNOR Lin*
<img width="1480" height="1022" alt="TNOR_Lin_schematic" src="https://github.com/user-attachments/assets/1ffafc3b-be38-4c8e-8429-c3c427a6e8ae" />

