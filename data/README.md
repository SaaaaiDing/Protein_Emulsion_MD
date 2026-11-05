# Original analysis exports

Each `peptide1`–`peptide4` directory contains three unmodified GROMACS XVG text files. Lines beginning with `#` or `@` contain provenance, commands, labels and units; the remaining lines contain two numeric columns.

| File | First column | Second column | Interpretation |
| --- | --- | --- | --- |
| `rmsd.xvg` | Time, ns (0–100) | C-alpha RMSD, nm | C-alpha deviation after least-squares fitting to C-alpha atoms, as recorded in the header |
| `rmsf.xvg` | Original atom identifier | RMSF, nm | One C-alpha entry per peptide residue; atom identifiers are not sequential residue numbers |
| `rdf.xvg` | Distance r, nm | g(r), dimensionless | Oleic-acid radial distribution around the C-alpha reference selection |

Peptide identities and article labels are in [systems.csv](../systems.csv). All values are retained at the precision of the original exports. These are processed numerical outputs from the original simulations, not raw coordinate trajectories or newly calculated data. Figure 6 contains initial system images; the associated RMSD/RDF results appear in Figure 7, and RMSF in Supplementary Figure S3. No replicate trajectories are claimed by this release.
