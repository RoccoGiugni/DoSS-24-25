# DoSS-24-25
Material of the course Dynamics of Stellar Systems A.Y. 2024/25


FILE 1: `nbody.C'

The Code `nbody.C' is a simple stand-alone version of an N-body system with shared but
variable time steps, based on the fourth-order Hermite integration scheme.
For example, on a Linux system you can use the GNU g++ compiler, and simply type:
"g++ -o nbody nbody.C" to produce the executable "nbody".

To run type: "nbody -d X -e X -o X -t X < in.txt > out.txt". Where -d is the integration
step, -e the time interval at which an update is printed on terminal, -o the time interval
at which coordinates are printed in the output file, -t is the time of the simulation.
X stands for the chosen value. Arguments aren't mandatory to run the code. The input and
output file are "in.txt" and "out.txt". The input file must be write as follow:

	n_bodies
	initial_time
	m_1 x_1 y_1 z_1 vx_1 vy_1 vz_1
	...
	m_n x_n y_n z_n vx_n vy_n vz_n
	
where notation is quite intuitive.

To download the code and for further references go to:

	https://www.ids.ias.edu/~piet/act/comp/algorithms/starter


OTHER FILEs

The other files in the repository are quite straight forward python notebooks used to
solve various exercizes during the course.
