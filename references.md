# References

Every non-trivial parameter or formula used in the notebooks is grounded in one of these papers or standards (see each notebook's own References section for exactly which equation/table is used where). The PDFs themselves aren't included in this repository — most are behind IEEE copyright, so only the citations are listed here. All of them are reachable through their DOI, and one (`[VCSEL-70Gbps]`) is freely available on arXiv.

| Key | Paper | Link |
|---|---|---|
| `[RIS-VLC]` | B. Genoves Guzman, M. Morales Cespedes, V. P. Gil Jimenez, A. Garcia Armada, M. Brandt-Pearce, "Resource Allocation Exploiting Reflective Surfaces to Minimize the Outage Probability in VLC," *IEEE Trans. Wireless Commun.*, vol. 24, no. 7, pp. 5493-5507, July 2025. | [doi.org/10.1109/TWC.2025.3547648](https://doi.org/10.1109/TWC.2025.3547648) |
| `[VCSEL-Precoding]` | H. Safi, A. Ihsan, H. B. Eldeeb, B. Béchadergue, I. Tavakkolnia, H. Haas, "Energy-Efficient Precoding for Dense VCSEL-Based OWC Systems Under a Cooperative Broadcast Model," in *2025 IEEE Global Communications Conference (GLOBECOM)*. | [doi.org/10.1109/GLOBECOM59602.2025.11431781](https://doi.org/10.1109/GLOBECOM59602.2025.11431781) |
| `[Capacity-Bound]` | J.-B. Wang, Q.-S. Hu, J. Wang, M. Chen, J.-Y. Wang, "Tight Bounds on Channel Capacity for Dimmable Visible Light Communications," *J. Lightwave Technol.*, vol. 31, no. 23, pp. 3771-3779, Dec. 2013. | [doi.org/10.1109/JLT.2013.2286088](https://doi.org/10.1109/JLT.2013.2286088) |
| `[Eye-Safety]` | M. Dehghani Soltani, E. Sarbazi, N. Bamiedakis, P. de Souza, H. Kazemi, J. M. H. Elmirghani, I. H. White, R. V. Penty, H. Haas, M. Safari, "Safety Analysis for Laser-Based Optical Wireless Communications: A Tutorial," *Proc. IEEE*, vol. 110, no. 8, pp. 1045-1072, Aug. 2022. | [doi.org/10.1109/JPROC.2022.3181968](https://doi.org/10.1109/JPROC.2022.3181968) |
| `[VCSEL-70Gbps]` | H. Kazemi, I. N. O. Osahon, N. Ledentsov Jr., I. Titkov, N. Ledentsov, H. Haas, "Achieving 70 Gb/s Over A VCSEL-Based Optical Wireless Link Using A Multi-Mode Fiber-Coupled Receiver," 2025. | [arxiv.org/abs/2506.18864](https://arxiv.org/abs/2506.18864) |

Also cited inside some of the papers above, and used here as supporting context (not directly cited by equation number):

- H. Kazemi et al., "A Novel Terabit Grid-of-Beam Optical Wireless Multi-User Access Network With Beam Clustering" — the grid-of-beam architecture behind the "thousands of beams" discussion in the multi-cell notebook.
- M. D. Soltani et al., "Terabit Indoor Laser-based Wireless Communications: LiFi 2.0 for 6G" — the LiFi 2.0 / 6G vision mentioned in the introduction.
- C. Chen, D. Tsonev, H. Haas, "Joint Transmission in Indoor VLC Downlink Cellular Networks" — the joint-transmission technique modelled in the cooperation section.

Standards referenced directly (not academic papers, no DOI):

- **IEC 60825-1:2014** — laser eye-safety standard, used for the VCSEL's maximum permissible exposure / eye-safe transmit power.
- **EN 12464-1** — lighting standard, used for the LED's illuminance target (500 lux over the task area).
