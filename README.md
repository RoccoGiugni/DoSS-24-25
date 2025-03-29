# DoSS-24-25
Material of the course Dynamics of Stellar Systems A.Y. 2024/25
from the Master Degree in Astrophysics and Space Physics in Bicocca University, Milan.


FILE 1: `nbody'

The Code `nbody.C' is a simple stand-alone version of an N-body system with shared but
variable time steps, based on the fourth-order Hermite integration scheme.
For example, on a Linux system you can use the GNU g++ compiler, and simply type:
"g++ -o nbody nbody.C" to produce the executable "nbody".

To run type:

    nbody -d X -e X -o X -t X < in.txt > out.txt
    
where -d is the integration step, -e the time interval at which an update is printed on
terminal, -o is the time interval at which coordinates are printed in the output file, -t is
the time of the simulation. X stands for the chosen value. Arguments aren't mandatory to
run the code. The input and output file are "in.txt" and "out.txt".
The input file must be write as follow:

	n_bodies
	initial_time
	m_1 x_1 y_1 z_1 vx_1 vy_1 vz_1
	...
	m_n x_n y_n z_n vx_n vy_n vz_n
	
where notation is quite intuitive. The output file has the same configuration and file
with the same name will be rewritten at each execution.

To download the code and for further references go to:

	https://www.ids.ias.edu/~piet/act/comp/algorithms/starter

FILE 2: `3code'

On Linux systems the compilation is quite simple, though it can appear frightening. To
avoid errors follow the link at the end of the paragraph.

To run type:

	3code in=in.txt out=out.txt dtime=X eps=X theta=X tstop=X dtout=X
	
where dtime is the integration step, eps is the smoothing length (used to avoid two body interactions), theta is the force accuracy angle (used to compute the volumes where p.cles
are considered as a whole), tstop is the time of the simulation, dtout is the time interval at which coordinates are printed in the output file. The input and output file are "in.txt"
and "out.txt".

The input file must be write as follow:

	n_bodies
	n_dim
	initial_time
	m_1
	...
	m_n
	x_1 y_1 z_1
	...
	x_n y_n z_n
	vx_1 vy_1 vz_1
	...
	vx_n vy_n vz_n
	
where notation is quite intuitive. The output file has the same configuration and file
with the same name will be appended at each execution.

To download the code and for further references go to:

	http://www.ifa.hawaii.edu/faculty/barnes/treecode/treeguide.html
	
Note that being redirected to another page is highly probable. The issue can be easily
solved writing "legacy" instead of "www", as follow:

	http://legacy.ifa.hawaii.edu/faculty/barnes/treecode/treeguide.html

OTHER FILEs

The other files in the repository are quite straight forward python notebooks used to
solve various exercizes during the course.
