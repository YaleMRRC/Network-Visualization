# NetworkVisualization
This code provides a framework for the network visualization of functional connectivity matrices.
### Inputs
1. The first input ('M') is a pre-calculated n x c x p x p matrix containing group-level connectivity matrices
   for all conditions and scan sessions, where n = number of re-scans for each condition, 
   c = number of conditions, and p = number of nodes in the chosen brain atlas.
   Each element (nn,cc,i,j) in these matrices represents the correlation between the BOLD timecourses
   of nodes i and j during a single fMRI session nn with condition cc. 

2. The second input ('networks') is the p x 1 vector of node-to-network allegiances. Each element (i) in this vector shows the network that node i is assigned to.


### Outputs
The functional connecitivity matrix is visualized as a network in the browser. See the Figure below for an example:

<center>
<img src="/images/cpm.svg"/>
</center>

### License
Copyright &copy; 2018, Mehraveh Salehi. This code is released under the terms of the GNU GPL v2. 
