# Compatibility Warning
Read if you wish to recreate the provided schematics:

**You need**: tsmc18rf technology library, Stanford CNFET models, Cadence Virtuoso, original parameters from references.

The exact parameters (n,m) for each CNFET are not provided and must be found from original sources of the designs. 

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

<table>
  <tr>
    <th align="center">STI Saketh</th>
    <th align="center">STI Jaber</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="STI_Saketh_inner" src="https://github.com/user-attachments/assets/bcddb95f-6876-4971-82e2-6e2f9a27a13a" /></td>
    <td align="center"><img width="400" alt="STI_Jaber_inner" src="https://github.com/user-attachments/assets/cb1158dc-ebcc-43dc-ba90-82cb48f2cc62" /></td>
  </tr>
  <tr>
    <th align="center">STI Lin</th>
    <th align="center">STI Trans Graph</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="STI_Lin_schematic" src="https://github.com/user-attachments/assets/aba66fa0-4351-4acf-a6cb-6dcd35baaad0" /></td>
    <td align="center"><img width="400" alt="STI_Jaber_trans_thick-1" src="https://github.com/user-attachments/assets/32a923f7-f178-4516-a97c-7bbe69675584" /></td>
  </tr>
</table>

### TNAND Gate

<table>
  <tr>
    <th align="center">TNAND Jaber</th>
    <th align="center">TNAND Lin</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="TNAND_Jaber_withsubcircuits" src="https://github.com/user-attachments/assets/52cdd6b9-9421-4b59-ad3f-7bc7d230056b" /></td>
    <td align="center"><img width="400" alt="TNAND_Lin_schematic" src="https://github.com/user-attachments/assets/d1d6a989-e646-4c4e-823e-4c76e70b385d" /></td>
  </tr>
  <tr>
    <th align="center" colspan="2">TNAND Graph</th>
  </tr>
  <tr>
    <td align="center" colspan="2"><img width="600" alt="TNAND_Lin_graph-1" src="https://github.com/user-attachments/assets/d31f1f8c-f841-4797-ba37-12d9678a69ca" /></td>
  </tr>
</table>

### TNOR Gate

<table>
  <tr>
    <th align="center">TNOR Lin</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="TNOR_Lin_schematic" src="https://github.com/user-attachments/assets/1ffafc3b-be38-4c8e-8429-c3c427a6e8ae" /></td>
  </tr>
</table>

### TDecoder

<table>
  <tr>
    <th align="center">TDecoder Jaber</th>
    <th align="center">TDecoder Lin</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="Tdecoder_Jaber_inner_schematic" src="https://github.com/user-attachments/assets/34004679-c405-41f1-a4e4-8fcea04c50b0" /></td>
    <td align="center"><img width="400" alt="Tdecoder_Lin_schematic" src="https://github.com/user-attachments/assets/02c5f0d8-1e30-484e-942e-df41e486be14" /></td>
  </tr>
  <tr>
    <th align="center" colspan="2">TDecoder Graph</th>
  </tr>
  <tr>
    <td align="center" colspan="2"><img width="600" alt="Tdecoder_Jaber_graph-1" src="https://github.com/user-attachments/assets/a7a061a3-d780-44a0-ad1e-4aa2715dbc90" /></td>
  </tr>
</table>

### Ternary Half Adder

<table>
  <tr>
    <th align="center">THA Lin</th>
    <th align="center">THA Jaber</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="THA_Lin_schematic" src="https://github.com/user-attachments/assets/c0ce0d91-5d81-4cb7-ab5a-0d01d7c1f8cc" /></td>
    <td align="center"><img width="400" alt="THA_Jaber_schematic" src="https://github.com/user-attachments/assets/5a9960d9-f27c-4009-906f-69df29f40883" /></td>
  </tr>
  <tr>
    <th align="center">Proposed THA</th>
    <th align="center">THA Graph</th>
  </tr>
  <tr>
    <td align="center"><img width="400" alt="proposed_THA" src="https://github.com/user-attachments/assets/0912dc43-8eef-49bc-8d2b-ac70f42029f7" /></td>
    <td align="center"><img width="400" alt="THA_Jaber_graph-1" src="https://github.com/user-attachments/assets/f296965b-df93-4166-8889-27990e9d9dab" /></td>
  </tr>
</table>

# Some Delay Data:

### TNAND Delay Analysis

<table>
  <tr>
    <th align="center">Design</th>
    <th align="center">Rise Time</th>
    <th align="center">Fall Time</th>
  </tr>
  <tr>
    <td align="center"><b>Jaber</b></td>
    <td><img width="400" alt="TNAND_jaber_delay_rise" src="https://github.com/user-attachments/assets/1aa29bef-fe62-47a0-af74-0068b05b7a65" /></td>
    <td><img width="400" alt="TNAND_jaber_delay_fall" src="https://github.com/user-attachments/assets/959cdca4-675d-4061-9e5b-9c0df52ab19a" /></td>
  </tr>
  <tr>
    <td align="center"><b>Lin</b></td>
    <td><img width="400" alt="TNAND_Lin_delay_rise" src="https://github.com/user-attachments/assets/2a5dbbb0-676f-4be0-9919-6015369ed46d" /></td>
    <td><img width="400" alt="TNAND_Lin_delay_fall" src="https://github.com/user-attachments/assets/6866b6c3-941e-4d8a-97fe-2be386b77356" /></td>
  </tr>
</table>


### STI Delay Profiles

<table>
  <tr>
    <th align="center">SIT Rise Time (Jaber)</th>
    <th align="center">SIT Fall Time (Jaber)</th>
  </tr>
  <tr>
    <td><img width="400" alt="STI_Jaber_delay_rise" src="https://github.com/user-attachments/assets/8366055e-5073-4cfb-bdc1-eba179c1fefb" /></td>
    <td><img width="400" alt="STI_Jaber_delay_fall" src="https://github.com/user-attachments/assets/06068199-9363-4318-a8e4-d7c28481fd7c" /></td>
  </tr>
</table>

### THA Jaber

<table>
  <tr>
    <th align="center">Sum</th>
    <th align="center">Carry</th>
  </tr>
  <tr>
    <td align="center">
      <b>Rise</b><br>
      <img width="400" src="https://github.com/user-attachments/assets/66262c47-3f1c-4a0a-bb2f-e9195ba35059" />
    </td>
    <td align="center">
      <b>Rise</b><br>
      <img width="400" src="https://github.com/user-attachments/assets/076bebc3-2fc7-44ec-ba03-caa4b27fdc85" />
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>Fall</b><br>
      <img width="400" src="https://github.com/user-attachments/assets/890589e0-98e6-4c1e-b3bc-22c9ece97fc5" />
    </td>
    <td align="center">
      <b>Fall</b><br>
      <img width="400" src="https://github.com/user-attachments/assets/95db600d-0d48-4536-bf88-271c268c8fb3" />
    </td>
  </tr>
</table>

### Proposed THA

<table>
  <tr>
    <th align="center">Sum</th>
    <th align="center">Carry</th>
  </tr>
  <tr>
    <td align="center">
      <b>Rise</b><br>
      <img width="400" alt="proposedTHA_sum_rise" src="https://github.com/user-attachments/assets/c6eccc24-c630-4809-8b82-ac51087c2186" />
    </td>
    <td align="center">
      <b>Rise</b><br>
      <img width="400" alt="proposedTHA_carry_rise" src="https://github.com/user-attachments/assets/86fed8d3-e012-43e7-bced-5aa641347406" />
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>Fall</b><br>
      <img width="400" alt="proposedTHA_sum_fall" src="https://github.com/user-attachments/assets/1532e240-c441-4ef9-8664-1324ed68a844" />
    </td>
    <td align="center">
      <b>Fall</b><br>
      <img width="400" alt="proposedTHA_carry_fall" src="https://github.com/user-attachments/assets/b9711452-674a-4af7-8571-334aaf90b56f" />
    </td>
  </tr>
</table>

