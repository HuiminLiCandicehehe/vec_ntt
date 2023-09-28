# Customized Vector Extensions for CRYSTALS-Kyber
RISC-V  Vector extensions for NTT
Repository code to support paper “Li H, Mentens N, Picek S. A scalable SIMD RISC-V based processor with customized vector extensions for CRYSTALS-kyber[C]//Proceedings of the 59th ACM/IEEE Design Automation Conference. 2022: 733-738.”
Link to the paper: https://dl.acm.org/doi/pdf/10.1145/3489517.3530552

## Scalablity
Change LaneNum （the element number）for each vector register: located in top_artya7.sv

## Work as the pure SIMD processor
Delete or comment the about "`ifdef VEC_CPU  ... `endif"

## RISC-V GNU Compiler Toolchain
We first used the toolchain: https://github.com/riscv-collab/riscv-gnu-toolchain/tree/rvv-intrinsic
Then later we found the developers had already deleted the link and published a new link：https://github.com/riscv-collab/riscv-gnu-toolchain/tree/rvv-next.

## Vivado Version
Vivado 2019.2
New versions also support if IPs are updated

## Ibex Version
The ibex core was sourced from the GitHub repository in April 2021.


## References

If you use this code, please consider citing:

@inproceedings{li2022scalable,
  title={A scalable SIMD RISC-V based processor with customized vector extensions for CRYSTALS-kyber},
  author={Li, Huimin and Mentens, Nele and Picek, Stjepan},
  booktitle={Proceedings of the 59th ACM/IEEE Design Automation Conference},
  pages={733--738},
  year={2022}
}
