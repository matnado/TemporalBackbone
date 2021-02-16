# A tool to detect the backbone in temporal networks

The computational time is O(N_E T^2), where N_E are the number unique edges in the network and T the number of time steps.

For sparse networks (like most of the large networks), the computational time is O(N T^2)
    
Input: 
- pandas dataframe with three columns: ***node1, node2, time*** *(order is important)*
- Minimum length of the interval: ***default 1 day** (time step is taken from the data)*
- whether the network is directed or not: ***default True***
- whether to use the Bonferroni correction: ***default True***
- threshold to determine the significance of a link: ***default 0.01***
    
Output:
- list with the significant links    


### Please cite

The methodology is first introduced in 
*Nadini, M., Bongiorno, C., Rizzo, A., & Porfiri, M. (2020). **Detecting network backbones against time variations in node properties.** Nonlinear Dynamics, 99(1), 855-878.*
    
Then was deemed as appropriate for large temporal networks, having a good trade-off between false positives and false negatives. See
*Nadini, M., Rizzo, A., & Porfiri, M. (2020). **Reconstructing irreducible links in temporal networks: which tool to choose depends on the network size.** Journal of Physics: Complexity, 1(1), 015001.*
    
